    ---
标题: "educationIdentitySynchronizationConfiguration 资源类型" 说明: "所有学校数据配置文件标识同步配置的抽象基类。 派生类定义用于同步标识的行为。 以下是派生类型。
author: "mmast-msft" 使用: 正常毫秒: "教育版"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

所有学校数据配置文件标识同步配置的摘要基类。 派生类定义用于同步标识的行为。 以下是派生类型。

## <a name="derived-types"></a>派生类型
| 类型 | 说明 |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | 使用此类型可匹配 azure Active Directory (azure AD) 中的现有用户帐户。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | 使用此类型在 Azure AD 中创建新用户帐户。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

