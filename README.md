 using System;

class AlgebraicExpression
{
    private Polynomial numerator;
    private Polynomial denominator;

    public AlgebraicExpression(Polynomial numerator, Polynomial denominator)
    {
        this.numerator = numerator;
        this.denominator = denominator;
    }

    public AlgebraicExpression(int[] numeratorCoefficients, int[] denominatorCoefficients)
    {
        this.numerator = new Polynomial(numeratorCoefficients);
        this.denominator = new Polynomial(denominatorCoefficients);
    }

    public double CalculateValue(double x)
    {
        if (denominator.Evaluate(x) == 0)
        {
            Console.WriteLine("Ошибка: деление на ноль");
            return 0;
        }
        return numerator.Evaluate(x) / denominator.Evaluate(x);
    }
}

class Polynomial
{
    private int[] coefficients;

    public Polynomial(int[] coefficients)
    {
        this.coefficients = coefficients;
    }

    public double Evaluate(double x)
    {
        double result = 0;
        for (int i = 0; i < coefficients.Length; i++)
        {
            result += coefficients[i] * Math.Pow(x, i);
        }
        return result;
    }
}

class Program
{
    static void Main()
    {
        int[] numeratorCoefficients = { 1, 2, 3 }; // Пример коэффициентов для числителя
        int[] denominatorCoefficients = { 4, 5 }; // Пример коэффициентов для знаменателя

        AlgebraicExpression expression = new AlgebraicExpression(numeratorCoefficients, denominatorCoefficients);

        double x = 2.5; // Пример значения x
        double result = expression.CalculateValue(x);

        Console.WriteLine($"Значение выражения при x = {x}: {result}");
    }
}using System;

class AlgebraicExpression
{
    private Polynomial numerator;
    private Polynomial denominator;

    public AlgebraicExpression(Polynomial numerator, Polynomial denominator)
    {
        this.numerator = numerator;
        this.denominator = denominator;
    }

    public AlgebraicExpression(int[] numeratorCoefficients, int[] denominatorCoefficients)
    {
        this.numerator = new Polynomial(numeratorCoefficients);
        this.denominator = new Polynomial(denominatorCoefficients);
    }

    public double CalculateValue(double x)
    {
        if (denominator.Evaluate(x) == 0)
        {
            Console.WriteLine("Ошибка: деление на ноль");
            return 0;
        }
        return numerator.Evaluate(x) / denominator.Evaluate(x);
    }
}

class Polynomial
{
    private int[] coefficients;

    public Polynomial(int[] coefficients)
    {
        this.coefficients = coefficients;
    }

    public double Evaluate(double x)
    {
        double result = 0;
        for (int i = 0; i < coefficients.Length; i++)
        {
            result += coefficients[i] * Math.Pow(x, i);
        }
        return result;
    }
}

class Program
{
    static void Main()
    {
        int[] numeratorCoefficients = { 1, 2, 3 }; // Пример коэффициентов для числителя
        int[] denominatorCoefficients = { 4, 5 }; // Пример коэффициентов для знаменателя

        AlgebraicExpression expression = new AlgebraicExpression(numeratorCoefficients, denominatorCoefficients);

        double x = 2.5; // Пример значения x
        double result = expression.CalculateValue(x);

        Console.WriteLine($"Значение выражения при x = {x}: {result}");
    }
}using System;

class AlgebraicExpression
{
    private Polynomial numerator;
    private Polynomial denominator;

    public AlgebraicExpression(Polynomial numerator, Polynomial denominator)
    {
        this.numerator = numerator;
        this.denominator = denominator;
    }

    public AlgebraicExpression(int[] numeratorCoefficients, int[] denominatorCoefficients)
    {
        this.numerator = new Polynomial(numeratorCoefficients);
        this.denominator = new Polynomial(denominatorCoefficients);
    }

    public double CalculateValue(double x)
    {
        if (denominator.Evaluate(x) == 0)
        {
            Console.WriteLine("Ошибка: деление на ноль");
            return 0;
        }
        return numerator.Evaluate(x) / denominator.Evaluate(x);
    }
}

class Polynomial
{
    private int[] coefficients;

    public Polynomial(int[] coefficients)
    {
        this.coefficients = coefficients;
    }

    public double Evaluate(double x)
    {
        double result = 0;
        for (int i = 0; i < coefficients.Length; i++)
        {
            result += coefficients[i] * Math.Pow(x, i);
        }
        return result;
    }
}

class Program
{
    static void Main()
    {
        int[] numeratorCoefficients = { 1, 2, 3 }; // Пример коэффициентов для числителя
        int[] denominatorCoefficients = { 4, 5 }; // Пример коэффициентов для знаменателя

        AlgebraicExpression expression = new AlgebraicExpression(numeratorCoefficients, denominatorCoefficients);

        double x = 2.5; // Пример значения x
        double result = expression.CalculateValue(x);

        Console.WriteLine($"Значение выражения при x = {x}: {result}");
    }
}
