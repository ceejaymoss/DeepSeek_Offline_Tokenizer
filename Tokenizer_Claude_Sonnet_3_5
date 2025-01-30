#visit https://token-counter.app/anthropic/claude-3.5-sonnet
# input your text into the chat box and output a token count

# Define cost constants
Input = 3
Prompt_coaching_write = 3.75
Prompt_coaching_read = 0.3
one_mill_tokens_output = 15

# Input your token count
token_count = 1534

# Calculate costs
token_cost_cache_hit = (token_count * one_mill_tokens_output * Input * Prompt_coaching_read) / 1_000_000
token_cost_cache_miss = (token_count * one_mill_tokens_output * Input * Prompt_coaching_write) / 1_000_000

print(f"Token count: {token_count}")
print(f"Cache hit cost (USD): ${token_cost_cache_hit:.6f}")
print(f"Cache miss cost (USD): ${token_cost_cache_miss:.6f}")

# Optional: Show cost per million tokens
print(f"\nCost per million tokens:")
print(f"Cache hit: ${one_mill_tokens_output * Prompt_coaching_read:.6f}")
print(f"Cache miss: ${one_mill_tokens_output * Prompt_coaching_write:.6f}")
