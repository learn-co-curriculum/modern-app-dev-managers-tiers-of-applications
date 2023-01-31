# Tiers of Application

## Learning Goals

- Explain the concept of a tier.
- Give an overview of the different tiers of applications.

## What is a Tier?

A tier is a physical and logical separation of components in an application or
service. Components are units designed to perform specific functions. Some
common components of a web service are:

- Database: Stores, manages, and queries data.
- Client: The user’s system. This can be a mobile phone, laptop, or desktop. The
  UI is presented here too.
- Backend application server: Handles client requests, manages messages between
  different components, and contains business logic.

Both a client and a server are computers. We use different names to signify
their different roles in an application.

## Single-tier Application

A single-tier application runs the user interface, backend business logic, and
the database in the same machine. For example, offline games, office suites,
notes apps.

The main benefit of this type of application is the lack of any network latency
(time taken to receive a response from a service) which makes it very fast.
Additionally, it has improved privacy since all user data is stored on the
client’s system.

One of the major disadvantage is that the developers have no control over the
software once it’s been sold to the client which means that they cannot provide
any updates, security patches, or features. The performance of the application
is also heavily reliant on the client’s system performance capability.

## Two-tier Application

This kind of application has a client and a server. The client contains the user
interface and the backend business logic on the same machine. The server
contains the database running on a different machine.

![Untitled](https://curriculum-content.s3.amazonaws.com/modern-app-dev-managers-leadership/tiers-of-applications/01.png)

For certain applications, it’s fine if the user has access to the business logic
on their machine. For example, a planner application can store the logic for its
UI and data presentation on the client’s system while the actual data is stored
securely on the server. Most mobile apps are also good examples since all the
files are downloaded from an app store once and then the save data is synced
with a server.

Since we are making as few server calls as possible, less money is needed to run
the servers. If we want to separate the user interface and the business logic,
we can use another server for it and create a three-tier application.

## Three-tier Application

These applications separate their user interface, business logic, and database
into different physical machines.

![Untitled](https://curriculum-content.s3.amazonaws.com/modern-app-dev-managers-leadership/tiers-of-applications/02.png)

## N-tier Application

An n-tier application is one which has more than the three components we’ve been
discussing so far. These are far more complex and is out of the scope for this
course. Most large scale applications like Uber, Airbnb, social media
applications are n-tier applications.

## Benefits of Tiers

Two of the most well-known concepts in software engineering are:

1. **Single Responsibility Principle:** This means giving a specific
   responsibility to a component and allowing it focus on performing that
   responsibility efficiently. Resources on a
2. Separation of Concerns: This indicates that components are loosely, i.e.,
   making changes to one component won’t affect another component’s
   functionality.

Using tiered applications allows us to use both of these concepts effectively
which allows us to create applications that are more maintainable, extensible,
and cost effective.

## Conclusion

In this lesson, we learned about the core components in applications, how we can
separate them into different tiers, and why we would want to do that.
