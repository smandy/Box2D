set(LIBRARY_FILES Box2D/Common/b2BlockAllocator.h Box2D/Common/b2BlockAllocator.cpp Box2D/Common/b2Math.h Box2D/Common/b2Timer.cpp Box2D/Common/b2Draw.h Box2D/Common/b2StackAllocator.cpp Box2D/Common/b2Settings.cpp Box2D/Common/b2Draw.cpp Box2D/Common/b2GrowableStack.h Box2D/Common/b2StackAllocator.h Box2D/Common/b2Settings.h Box2D/Common/b2Timer.h Box2D/Common/b2Math.cpp Box2D/Box2D.h Box2D/Dynamics/b2Island.h Box2D/Dynamics/Contacts/b2EdgeAndPolygonContact.h Box2D/Dynamics/Contacts/b2Contact.h Box2D/Dynamics/Contacts/b2PolygonAndCircleContact.cpp Box2D/Dynamics/Contacts/b2EdgeAndCircleContact.cpp Box2D/Dynamics/Contacts/b2EdgeAndPolygonContact.cpp Box2D/Dynamics/Contacts/b2Contact.cpp Box2D/Dynamics/Contacts/b2ContactSolver.h Box2D/Dynamics/Contacts/b2ChainAndPolygonContact.cpp Box2D/Dynamics/Contacts/b2PolygonContact.cpp Box2D/Dynamics/Contacts/b2PolygonContact.h Box2D/Dynamics/Contacts/b2CircleContact.h Box2D/Dynamics/Contacts/b2ChainAndPolygonContact.h Box2D/Dynamics/Contacts/b2ChainAndCircleContact.cpp Box2D/Dynamics/Contacts/b2PolygonAndCircleContact.h Box2D/Dynamics/Contacts/b2CircleContact.cpp Box2D/Dynamics/Contacts/b2EdgeAndCircleContact.h Box2D/Dynamics/Contacts/b2ChainAndCircleContact.h Box2D/Dynamics/Contacts/b2ContactSolver.cpp Box2D/Dynamics/b2World.cpp Box2D/Dynamics/b2Island.cpp Box2D/Dynamics/b2Fixture.h Box2D/Dynamics/b2Body.cpp Box2D/Dynamics/b2Fixture.cpp Box2D/Dynamics/b2WorldCallbacks.h Box2D/Dynamics/b2WorldCallbacks.cpp Box2D/Dynamics/b2ContactManager.h Box2D/Dynamics/b2World.h Box2D/Dynamics/b2ContactManager.cpp Box2D/Dynamics/b2Body.h Box2D/Dynamics/b2TimeStep.h Box2D/Dynamics/Joints/b2GearJoint.cpp Box2D/Dynamics/Joints/b2FrictionJoint.cpp Box2D/Dynamics/Joints/b2WeldJoint.cpp Box2D/Dynamics/Joints/b2PulleyJoint.h Box2D/Dynamics/Joints/b2FrictionJoint.h Box2D/Dynamics/Joints/b2WheelJoint.cpp Box2D/Dynamics/Joints/b2MotorJoint.h Box2D/Dynamics/Joints/b2WheelJoint.h Box2D/Dynamics/Joints/b2PrismaticJoint.h Box2D/Dynamics/Joints/b2WeldJoint.h Box2D/Dynamics/Joints/b2RevoluteJoint.h Box2D/Dynamics/Joints/b2DistanceJoint.h Box2D/Dynamics/Joints/b2RevoluteJoint.cpp Box2D/Dynamics/Joints/b2GearJoint.h Box2D/Dynamics/Joints/b2PulleyJoint.cpp Box2D/Dynamics/Joints/b2MouseJoint.cpp Box2D/Dynamics/Joints/b2Joint.h Box2D/Dynamics/Joints/b2PrismaticJoint.cpp Box2D/Dynamics/Joints/b2MotorJoint.cpp Box2D/Dynamics/Joints/b2RopeJoint.h Box2D/Dynamics/Joints/b2MouseJoint.h Box2D/Dynamics/Joints/b2Joint.cpp Box2D/Dynamics/Joints/b2RopeJoint.cpp Box2D/Dynamics/Joints/b2DistanceJoint.cpp Box2D/Rope/b2Rope.h Box2D/Rope/b2Rope.cpp Box2D/Collision/b2BroadPhase.h Box2D/Collision/b2Distance.h Box2D/Collision/b2TimeOfImpact.cpp Box2D/Collision/b2DynamicTree.h Box2D/Collision/b2CollideCircle.cpp Box2D/Collision/b2CollidePolygon.cpp Box2D/Collision/Shapes/b2Shape.h Box2D/Collision/Shapes/b2ChainShape.cpp Box2D/Collision/Shapes/b2PolygonShape.cpp Box2D/Collision/Shapes/b2ChainShape.h Box2D/Collision/Shapes/b2CircleShape.h Box2D/Collision/Shapes/b2EdgeShape.h Box2D/Collision/Shapes/b2PolygonShape.h Box2D/Collision/Shapes/b2EdgeShape.cpp Box2D/Collision/Shapes/b2CircleShape.cpp Box2D/Collision/b2Collision.cpp Box2D/Collision/b2TimeOfImpact.h Box2D/Collision/b2CollideEdge.cpp Box2D/Collision/b2Distance.cpp Box2D/Collision/b2BroadPhase.cpp Box2D/Collision/b2DynamicTree.cpp Box2D/Collision/b2Collision.h)

include_directories(BEFORE . )
add_library( box2d SHARED ${LIBRARY_FILES})


add_executable( testbed Testbed/Framework/Main.cpp
                        Testbed/Framework/Test.h
                        Testbed/Framework/Test.cpp
                        Testbed/Framework/DebugDraw.h
                        Testbed/Framework/DebugDraw.cpp
                        Testbed/Tests/Gears.h
                        Testbed/Tests/ConvexHull.h
                        Testbed/Tests/Pyramid.h
                        Testbed/Tests/DumpShell.h
                        Testbed/Tests/HeavyOnLight.h
                        Testbed/Tests/PolyCollision.h
                        Testbed/Tests/MotorJoint.h
                        Testbed/Tests/BasicSliderCrank.h
                        Testbed/Tests/Confined.h Testbed/Tests/Chain.h
                        Testbed/Tests/TheoJansen.h
                        Testbed/Tests/Bridge.h Testbed/Tests/Pulleys.h
                        Testbed/Tests/DynamicTreeTest.h
                        Testbed/Tests/Revolute.h Testbed/Tests/Car.h
                        Testbed/Tests/SensorTest.h
                        Testbed/Tests/EdgeShapes.h
                        Testbed/Tests/Skier.h
                        Testbed/Tests/ApplyForce.h
                        Testbed/Tests/PolyShapes.h
                        Testbed/Tests/VerticalStack.h
                        Testbed/Tests/Prismatic.h Testbed/Tests/Rope.h
                        Testbed/Tests/EdgeTest.h
                        Testbed/Tests/BulletTest.h
                        Testbed/Tests/TestEntries.cpp
                        Testbed/Tests/AddPair.h
                        Testbed/Tests/RayCast.h
                        Testbed/Tests/chainProblem.h
                        Testbed/Tests/TimeOfImpact.h
                        Testbed/Tests/Pinball.h
                        Testbed/Tests/SphereStack.h
                        Testbed/Tests/CollisionFiltering.h
                        Testbed/Tests/CollisionProcessing.h
                        Testbed/Tests/CompoundShapes.h
                        Testbed/Tests/Tumbler.h
                        Testbed/Tests/ConveyorBelt.h
                        Testbed/Tests/CharacterCollision.h
                        Testbed/Tests/Breakable.h
                        Testbed/Tests/RopeJoint.h
                        Testbed/Tests/SliderCrank.h
                        Testbed/Tests/OneSidedPlatform.h
                        Testbed/Tests/VaryingFriction.h
                        Testbed/Tests/VaryingRestitution.h
                        Testbed/Tests/Dominos.h
                        Testbed/Tests/ContinuousTest.h
                        Testbed/Tests/BodyTypes.h
                        Testbed/Tests/HeavyOnLightTwo.h
                        Testbed/Tests/Tiles.h
                        Testbed/Tests/DistanceTest.h
                        Testbed/Tests/Mobile.h Testbed/Tests/Web.h
                        Testbed/Tests/Cantilever.h
                        Testbed/Tests/MobileBalanced.h
                        Testbed/Tests/ShapeEditing.h)

set(GLEW_SOURCES glew/wglew.h
glew/glxew.h
glew/glew.c
glew/glew.h)


add_library(glew ${GLEW_SOURCES})


set(GLFW_SOURCES glfw/internal.h glfw/glfw_config.h glfw/glfw3.h
                 glfw/glfw3native.h glfw/context.c glfw/init.c
                 glfw/input.c glfw/monitor.c glfw/vulkan.c
                 glfw/window.c glfw/x11_platform.h glfw/xkb_unicode.h
                 glfw/linux_joystick.h glfw/posix_time.h
                 glfw/posix_tls.h glfw/glx_context.h
                 glfw/egl_context.h glfw/x11_init.c glfw/x11_monitor.c
                 glfw/x11_window.c glfw/glx_context.h
                 glfw/glx_context.c glfw/glext.h glfw/xkb_unicode.c
                 glfw/linux_joystick.c glfw/posix_time.c
                 glfw/posix_tls.c glfw/glx_context.c
                 glfw/egl_context.c)



               set(imgui_sources imgui/imgui.h imgui/stb_textedit.h imgui/stb_rect_pack.h imgui/imgui_demo.cpp imgui/imgui.cpp imgui/imgui_draw.cpp imgui/imgui_impl_glfw_gl3.cpp imgui/imgui_internal.h imgui/imconfig.h imgui/stb_truetype.h imgui/imgui_impl_glfw_gl3.h )

add_library(imgui ${imgui_sources})               

add_library(glfw ${GLFW_SOURCES})

target_link_libraries(testbed box2d glew imgui GL GLU GLEW glfw dl X11 Xrandr Xinerama Xcursor pthread)

install(TARGETS testbed
        RUNTIME DESTINATION bin
        LIBRARY DESTINATION lib
        ARCHIVE DESTINATION lib/static)
