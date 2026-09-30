import random
import time

def ultimate_match_calculator():
    print("=" * 60)
    print("🔥 ULTIMATE CRUSH & VIBE MATCH CALCULATOR (Python Edition) 🔥")
    print("=" * 60)
    
    
    name1 = input("👤 Enter your name.: ")
    name2 = input("💖 Crush name: ")
    
    print("\n🔮 The data has been verified against the forces of the universe. ")
    time.sleep(2) 
    
    combined_names = name1.strip().lower() + name2.strip().lower()
    score = sum(ord(char) for char in combined_names) % 101
    
    print("\n" + "=" * 60)
    print(f"✨ Result: {name1} ❤️ {name2}")
    print(f"📊 Match percentage: {score}%")
    print("-" * 60)
    
    if score >= 85:
        print("💎It's a perfect match! Looks like it's time to get the wedding rings ready! 😍💍")
    elif score >= 60:
        print("🔥 Great! If you give it a little effort, you can pull it off perfectly ! 😉🚀")
    elif score >= 40:
        print("⚖️ It seems a bit difficult, but you might not be able to work it out even by talking it over! 🤔")
    else:
        print("⚠️NOOOO broooo noo  😂")
        
    print("=" * 60)

if __name__ == "__main__":
    ultimate_match_calculator()
