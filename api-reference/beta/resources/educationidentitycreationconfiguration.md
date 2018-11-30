---
title: educationIdentityCreationConfiguration 资源类型
description: 创建学校数据配置文件标识上定义的设置。 这些身份包括学生和教师。 根据这些设置，将在目录中创建用户。
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048493"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

创建学校数据配置文件标识上定义的设置。 这些身份包括学生和教师。 根据这些设置，将在目录中创建用户。

> **注意：** 如果您有目录同步到本地之间的同步开启，Active Directory 和 Azure Active Directory (Azure AD)，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。

派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md)集合 |  设置要使用的每个用户类型的域的列表。  |


## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```