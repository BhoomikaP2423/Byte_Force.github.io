# Byte_Force.github.io
Problem Statement: Anxiety Detection Through Interaction Friction using AI

import { Link } from "react-router-dom";
import { Button } from "@/components/ui/button";
import { Activity, Brain, TouchpadIcon } from "lucide-react";

const Index = () => {
  return (
    <div className="min-h-screen bg-gradient-to-br from-background via-background to-secondary">
      <div className="container mx-auto px-4 py-16">
        {/* Hero Section */}
        <div className="text-center mb-16 animate-fade-in">
          <div className="inline-flex items-center justify-center w-20 h-20 rounded-full bg-primary/10 mb-6">
            <Brain className="w-10 h-10 text-primary" />
          </div>
          <h1 className="text-5xl md:text-6xl font-bold mb-6 bg-gradient-to-r from-primary to-accent bg-clip-text text-transparent">
            Anxiety Detection Through
            <br />
            Interaction Friction
          </h1>
          <p className="text-xl text-muted-foreground max-w-3xl mx-auto mb-8">
            When people are anxious, their device interactions become shaky—tapping slower, 
            scrolling repeatedly, unlocking hesitantly. We measure this friction in real time 
            to detect anxiety levels with unprecedented accuracy.
          </p>
          <div className="flex flex-col sm:flex-row gap-4 justify-center">
            <Link to="/test">
              <Button size="lg" className="text-lg px-8">
                Start Anxiety Test
              </Button>
            </Link>
            <Link to="/about">
              <Button size="lg" variant="outline" className="text-lg px-8">
                Learn More
              </Button>
            </Link>
          </div>
        </div>

        {/* Features Grid */}
        <div className="grid md:grid-cols-3 gap-8 mt-20">
          <div className="bg-card rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all border border-border">
            <div className="w-12 h-12 rounded-lg bg-primary/10 flex items-center justify-center mb-4">
              <TouchpadIcon className="w-6 h-6 text-primary" />
            </div>
            <h3 className="text-2xl font-semibold mb-3">Touch Analysis</h3>
            <p className="text-muted-foreground">
              Records tap patterns, pressure sensitivity, and rhythm variations to identify 
              interaction friction.
            </p>
          </div>

          <div className="bg-card rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all border border-border">
            <div className="w-12 h-12 rounded-lg bg-primary/10 flex items-center justify-center mb-4">
              <Activity className="w-6 h-6 text-primary" />
            </div>
            <h3 className="text-2xl font-semibold mb-3">Real-Time Metrics</h3>
            <p className="text-muted-foreground">
              Live anxiety meter visualizes your interaction patterns with instant feedback 
              and detailed analytics.
            </p>
          </div>

          <div className="bg-card rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all border border-border">
            <div className="w-12 h-12 rounded-lg bg-primary/10 flex items-center justify-center mb-4">
              <Brain className="w-6 h-6 text-primary" />
            </div>
            <h3 className="text-2xl font-semibold mb-3">Advanced Algorithm</h3>
            <p className="text-muted-foreground">
              Machine learning models analyze hesitation, repeat actions, and timing 
              inconsistencies to calculate anxiety levels.
            </p>
          </div>
        </div>

        {/* CTA Section */}
        <div className="mt-20 text-center bg-gradient-to-r from-primary/10 to-accent/10 rounded-3xl p-12 border border-primary/20">
          <h2 className="text-3xl font-bold mb-4">Ready to understand your interaction patterns?</h2>
          <p className="text-lg text-muted-foreground mb-6">
            Start your anxiety detection test now and see real-time results.
          </p>
          <Link to="/test">
            <Button size="lg" className="text-lg px-10">
              Begin Test
            </Button>
          </Link>
        </div>
      </div>
    </div>
  );
};

export default Index;
