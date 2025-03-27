# Navbar components

Welcome to my homemade navbar component, You can modify and redevelop it to make a better navbar.

## Example 1

![Navbar](/Assets/img/image.png)
If you want to get a navbar design like the one I made, you can copy the code below.

### HTML code

```
<nav class="bg-blue-100">
            <div class="flex flex-row flex-wrap justify-between items-center max-w-7xl mx-auto px-4">
                <div class="py-4">
                    <span class="text-2xl font-semibold">Navbar</span>
                </div>
                <div data-collapse-toggle="navbar-default" class="md:hidden flex items-center" aria-controls="navbar-default" onclick="toggleMenu()">
                    <i class="fa-solid fa-bars text-2xl"></i>
                </div>
                <div class="hidden @sm:h-[100vh] w-full md:block md:w-auto  flex items-center justify-center" id="navbar-default">
                    <ul class="flex text-lg flex-col p-2mt-4 rounded-lg md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0  dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
                        <li class="py-2 ">Service</li>
                        <li class="py-2">Projects</li>
                        <li class="py-2">Question</li>
                    </ul>
                </div>
            </div>
         </nav>
```

### JQuery version code

```
  function toggleMenu(){
            const menu = $("#navbar-default");
            menu.slideToggle('hidden');
        }
```

### Javascript version code

```
  function toggleMenu(){
            const menu = $("#navbar-default");
            menu.slideToggle('hidden');
        }
```

## Example 2

![Navbar](/Assets/img/Example2.png)
Do you need a navbar with a form? Of course we have a navbar with an input form only. Next there will be types of navbars that may be in line with your needs.

### HTML code

```
    <div class="example-2 mt-5">
         <nav class="bg-blue-400 text-white">
            <div class="flex flex-row flex-wrap justify-between items-center max-w-7xl mx-auto px-4">
                <div class="py-4">
                    <span class="text-2xl font-semibold">Navbar</span>
                </div>
                <div class="text-red-700 bg-white rounded-lg flex">
                    <input type="text" placeholder="Search..." class="px-4 py-2 focus:outline-none focus:ring-2 focus:ring-blue-500 rounded-l-lg">
                    <button class="bg-blue-500 text-white px-4 py-2 rounded-r-lg hover:bg-blue-600">
                        <i class="fa-solid fa-search"></i>
                    </button>
                </div>
            </div>
         </nav>
    </div>
```

## Example 3
Responsive navbar using dropdown

![Navbar](/Assets/img/Example3.png)

### HTML code
```
         <nav class="bg-blue-400 text-white">
            <div class="flex flex-row flex-wrap justify-between items-center max-w-7xl mx-auto px-4">
                <div class="py-4">
                    <span class="text-2xl font-semibold">Navbar</span>  
                </div>

                <div data-collapse-toggle="navbar-example-3" class="md:hidden flex items-center" aria-controls="navbar-example-3" onclick="navbarExample3()">
                    <i class="fa-solid fa-bars text-2xl"></i> 
                </div>

                <div class="hidden md:block md:w-auto  w-full flex md:flex-row text-start " id="navbar-example-3">
                    <ul class="flex md:flex-row gap-5 flex-col text-start">
                        <li>
                            <div class="relative dropdown-menu-example-3 ">
                                <button onclick="dropdown()" class="flex items-center hover:text-gray-200">
                                    <span>Menu</span>
                                    <i class="fa-solid fa-chevron-down"></i>
                                </button>
                                <div id="dropdownExample" class="hidden md:absolute md:w-48 md:shadow-lg mt-5 right-0 z-48 top-full mt-2 right-0 w-full rounded-lg">
                                    <ul class="py-2 text-gray-700">
                                        <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Profile</a></li>
                                        <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Settings</a></li>
                                        <li><a href="#" class="block px-4 py-2 hover:bg-gray-100">Logout</a></li>
                                    </ul>
                                </div>
                            </div>
                        </li>
                        <li class="hover:text-gray-200">
                            <a href="#" class="py-4">Service</a>
                        </li>
                    </ul>
                </div>
                
            </div>
         </nav>
```

### Jquery code
a