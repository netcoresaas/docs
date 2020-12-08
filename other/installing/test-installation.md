# 4. Test installation

### 1. Disable automatic database creation

If you haven't set your connection settings, open the Data/SystemDbContext.cs and Data/AppDbContext.cs files and comment the following line:

```csharp
// Database.EnsureCreated();
```

### 2. Run the app

Open the terminal at the root directory:

```text
$ dotnet run
```

Open [http://localhost:8080](http://localhost:8080)

### 3. Enable automatic database creation

Uncomment the lines mentioned in step 1.

### 4. All set

You're ready to configure your app:







