# Ejemplo para la introducción de Xamarin con FORMS. - Nivel 0

App para Windows (UWP, IOS y Android)

Aplicación con un botón, un variable que se usa como contador y una etiqueta que se pinta el resultado del contador.

Cada vez que se pulsa sobre el botón se actualiza el valor de la etiqueta (Label).

En la vista creamos el label y el botón.

  <StackLayout Padding="10"  HorizontalOptions="CenterAndExpand">
      <Label Text="0" FontSize="60" Margin="20" x:Name="etiqueta" TextColor="Green"/>
      <Button Clicked="Button_Clicked" Text="Contar"></Button>
    </StackLayout>
	

En el código detrás de la vista:
	
	int contador = 0;
	public HolaPage()
	{
		InitializeComponent();
	}

	private void Button_Clicked(object sender, EventArgs e)
	{
		contador++;
		etiqueta.Text = contador.ToString();
	}
	
	
Esta no es una buena forma de trabajar, ya veremos otros ejemplos más a delante.

Cualquiera duda contacta por twitter: @elbrinner

