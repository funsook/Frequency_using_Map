# Frequency_using_Map
package Frequency_using_Map;

import java.util.HashMap;

public class FrequencyUsingHashMap {
    public static void main(String[] args) {
        String str = "Hello world";
        HashMap<Character, Integer> map = new HashMap<>();
       
        for (char c : str.toCharArray()) {
        	if(c!=' ') {
            map.put(c, map.getOrDefault(c, 0) + 1);
        }
        }

        System.out.println(map);
    }
}
