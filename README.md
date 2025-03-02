# -Interactive-Quadratic-Visualizer
This project is an interactive tool built with Maple that allows users to explore how the coefficients a, b, and c of a quadratic function affect its graph. 
# Définir les paramètres pour une fonction quadratique
> restart;
> with(plots);

# Définir les coefficients
> a := 1;
> b := -2;
> c := 1;

# Créer des curseurs pour ajuster les coefficients
> Slider(a, -5..5, 0.1, "Coefficient a", "a");
> Slider(b, -5..5, 0.1, "Coefficient b", "b");
> Slider(c, -5..5, 0.1, "Coefficient c", "c");

# Fonction quadratique
> f := a*x^2 + b*x + c;

# Tracer la fonction en fonction des paramètres
> plot1 := plot(f, x=-10..10, title="Fonction quadratique", labels=["x", "f(x)"], color=blue);

# Afficher le graphique interactif
> display(plot1);
