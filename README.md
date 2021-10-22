# python-#用get方法来访问私有数据域
class A:
    def __init__(self,i):
        self.__i = i
    def geti(self):
        return self.__i
def main():
    a = A(5)
    print(a.geti())
main()
#1、第一个参数永远是 self ，并且调用时不用传递该参数
#2、在类中函数相互调用要加self
