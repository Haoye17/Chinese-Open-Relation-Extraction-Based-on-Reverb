# Chinese-Open-Relation-Extraction-Based-on-Reverb
A Chinese open relation extraction method based on Reverb, using POS tags to construct extraction rules.

## Example
### Input: List of sentences
sentences = ["德国总统高克。","高克访问中国。","习近平在上海视察。","习近平对埃及进行国事访问。","奥巴马毕业于哈佛大学。",
             "习近平主席和李克强总理接见普京。","习近平访问了美国和英国。","高克访问中国，并在同济大学发表演讲。"]
### Output: List of extracted triples
[{'sentence': '习近平对埃及进行国事访问。', 'arg1': '平对埃及', 'relation': '进行', 'arg2': '国事访问'}, {'sentence': '奥巴马毕业于哈佛大学。', 'arg1': '奥巴马', 'relation': '毕业于', 'arg2': '哈佛大学'}, {'sentence': '习近平主席和李克强总理接见普京。', 'arg1': '李克强总理', 'relation': '接见', 'arg2': '普京'}, {'sentence': '习近平访问了美国和英国。', 'arg1': '习近平', 'relation': '访问', 'arg2': '美国'}, {'sentence': '高克访问中国，并在同济大学发表演讲。', 'arg1': '中国', 'relation': '在同济大学发表', 'arg2': '演讲'}]

## Requirement
spacy

## Reference
Fader, A., Soderland, S., & Etzioni, O. (2011, July). Identifying relations for open information extraction. In Proceedings of the 2011 conference on empirical methods in natural language processing (pp. 1535-1545).
