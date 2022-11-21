# inherited-code
class BadLengthException : public std::exception
{
    private:
    int l=0;
    public:
    BadLengthException(int n) { l=n; }
    int what() { return l; }
};
