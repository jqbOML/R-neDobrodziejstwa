import matplotlib.pyplot as plt
import matplotlib.animation as animation


fig = plt.figure()
ax1 = fig.add_subplot(1,1,1)

def animate(i):
    data = open('plot_data.txt','r').read()
    lines = data.split('\n')
    xs = []
    ys = []
   
    for line in lines:
        x, y = line.split(',')    
        xs.append(float(x))
        ys.append(float(y))
    
    ax1.clear()
    ax1.plot(xs, ys)

    plt.xlabel('x_label_name')
    plt.ylabel('y_label_name')
    plt.title('Live graph with matplotlib')	
	
    
ani = animation.FuncAnimation(fig, animate, interval=1000) 
plt.show()
