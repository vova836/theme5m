using System;

class DistanceProblem
{
    public int CalculateDistance(int v1, int v2, int L)
    {
        int time = L / (v2 - v1);
        int distance = v2 * time;
        return distance;
    }
}

class Program
{
    static void Main()
    {
        int v1 = 10; // скорость велосипедиста
        int v2 = 20; // скорость мотоциклиста
        int L = 30; // расстояние между пунктами A и B

        DistanceProblem problem = new DistanceProblem();
        int distance = problem.CalculateDistance(v1, v2, L);

        Console.WriteLine("Мотоциклист догонит велосипедиста на расстоянии: " + distance + " км от пункта A.");
    }
}
