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
