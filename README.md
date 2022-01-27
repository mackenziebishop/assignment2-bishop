# assignment2-bishop
# Name: Mackenzie Bishop
## Favorite place to buy food: Casa Grande
Casa Grande is a Mexican restaurant in my home town. It's located off of our town square and is a family-owned business. Next door to it is the **Jackson Cafe**, which houses apartments above a small cafe that is one of the main hangout spots in town. On the other side, a German bistro, **Beethoven's**, is one of the oldest restaurants the town has.
## Directions from KCI + Recommendations
The closest airport to Casa Grande is Kansas City International Airport. Directions on how to get to the restaurant are posted below:

1. Get on I-29 S/US-71 S in May Township from NW 120th St

2. Follow I-29 S/US-71 S, I-635 S and I-35 S to KS-7 S/US-169 S/S Harrison St/S Woodland St in Olathe. Take exit 215 from I-35 S

3. Continue on KS-7 S/US-169 S. Drive to W Peoria St in Paola

###### Food Items I Would Recommend
- Fajita Quesadilla
- Espinaca Dip
- Pollo Casa Grande

## About Me
To learn more [about me](https://github.com/mackenziebishop/assignment2-bishop/blob/main/AboutMe.md), view the AboutMe.md file above!

## Sports + Recommendations
Sports are both fun to play and fun to watch! Below are some sports that I have played/watched that I recommend you try out for yourself!

| Name | Location | Cost |
| --- | --- | --- |
| Basketball | Park | $74 | 
| Softball | Park | $150 |
| Volleyball | Gym | $170 |

## Inspirational Quotes
> “Live as if you were to die tomorrow. Learn as if you were to live forever.” - _Mahatma Gandhi_\
> “Darkness cannot drive out darkness: only light can do that. Hate cannot drive out hate: only love can do that.” - _Martin Luther King Jr._

## Algorithms: Area of A Simple Polygon
According to [Wikipedia](https://en.wikipedia.org/wiki/Simple_polygon),mathematicians typically use "polygon" to refer only to the shape made up by the line segments, not the enclosed region, however some may use "polygon" to refer to a plane figure that is bounded by a closed path, composed of a finite sequence of straight line segments (i.e., by a closed polygonal chain). According to the definition in use, this boundary may or may not form part of the polygon itself. Below is a computational formula for [the area of a simple polygon](https://cp-algorithms.com/geometry/area-of-simple-polygon.html):
```
double area(const vector<point>& fig) {
    double res = 0;
    for (unsigned i = 0; i < fig.size(); i++) {
        point p = i ? fig[i - 1] : fig.back();
        point q = fig[i];
        res += (p.x - q.x) * (p.y + q.y);
    }
    return fabs(res) / 2;
}
```
