PUT top500_company_names
{
  "settings": {
    "number_of_shards": 1,
    "number_of_replicas": 0,
    "index": {
      "analysis": {
        "analyzer": {
          "ansj_analyzer_query": {
            "tokenizer": "ansj_tokenizer_query"
          },
          "ansj_analyzer_index": {
            "tokenizer": "ansj_tokenizer_index"
          }
        },
        "tokenizer": {
          "ansj_tokenizer_index": {
            "ambiguity": "",
            "stop": "",
            "synonyms": "",
            "isQuantifierRecognition": "true",
            "isRealName": "false",
            "type": "index_ansj",
            "isNameRecognition": "false",
            "isNumRecognition": "false",
            "dic": "dic"
          },
          "ansj_tokenizer_query": {
            "ambiguity": "",
            "stop": "",
            "synonyms": "",
            "isQuantifierRecognition": "true",
            "isRealName": "false",
            "type": "query_ansj",
            "isNameRecognition": "false",
            "isNumRecognition": "false",
            "dic": "dic"
          }
        }
      }
    }
  },
  "mappings": {
    "properties": {
      "name": {
        "type": "text",
        "analyzer": "ansj_analyzer_index",
        "search_analyzer": "ansj_analyzer_query"
      }
    }
  }
}
