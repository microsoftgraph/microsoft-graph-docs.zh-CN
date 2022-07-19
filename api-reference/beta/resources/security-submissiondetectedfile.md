---
title: submissionDetectedFile 资源类型
description: 表示威胁提交中检测到的文件的信息
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d12212968b55125776831b770f93b1e482162b3
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856668"
---
# <a name="submissiondetectedfile-resource-type"></a>submissionDetectedFile 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示威胁提交中检测到的文件的信息。

## <a name="properties"></a>属性
| 属性 | 类型   | Description    |
|:---------|:-------|:---------------|
| fileHash | String | 文件哈希。 |
| fileName | String | 文件名。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionDetectedFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionDetectedFile",
  "fileName": "String",
  "fileHash": "String"
}
```

