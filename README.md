public class Panchito extends GitHubUser {

  public Panchito() {
    super("Panchito", "Belgium");

    this.addLanguage("Java", "C#", "Javascript", "SQL", "PHP");
  }
}

public abstract class GitHubUser {

  private final String name;
  private final String country;

  private ArrayList<String> languages = new ArrayList<>();

  public GitHubUser(String name, String country) {
      this.name = name;
      this.country = country;
  }

  public void addLanguage(String... languages) {
    languages.addAll(languages);
  }
  
}
