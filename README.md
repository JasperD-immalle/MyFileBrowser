# MyFileBrowser

namespace MyFileBrowser
{

	class Program
	{
		static void Main(string[] args)
		{
			if (args.Length == 0)
			{

				Console.WriteLine("Geef een argument");

			}
			else
			{
				switch (args[0])
				{
					case "-c":
						ShowCurrentDirectory();
						Console.WriteLine("Alle files in current directory");
						break;
					case "-f":
						ShowAllFilesInCurrentDirectory();
						break;

					default:
						Console.WriteLine("Onbekend argument");
						break;

					case "-h":
						ShowHelp();
						break;

					case "-d":
						SubDirectories();
						Console.WriteLine("Alle SubDirectories in current directory");
						break;

				}
			}
		}

		static void ShowCurrentDirectory()
		{
			Console.WriteLine("Current Directory");
		}

		static void ShowAllFilesInCurrentDirectory()
		{
			Console.WriteLine("Alle files in current directory");
		}

		static void ShowHelp()
		{
			Console.WriteLine("Show help");
		}

		static void SubDirectories()
		{
			Console.WriteLine("Current SubDirectory");
		}

		public static void main()
		{

			string letters = "Dit zijn een aantal letters";
			int[] getallen = { 1, 2, 3, 4 };
			string[] woorden = { "Dit", "zijn", "een", "aantal", "woorden" };

			Console.WriteLine(letters);
			Console.WriteLine(woorden);
		}
	}
}
