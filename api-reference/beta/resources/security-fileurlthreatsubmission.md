---
title: fileUrlThreatSubmission 资源类型
description: 表示使用文件 URL 提交时创建的文件威胁提交对象。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b77f0fd8e8fb962546cd473bd3159ae7901c054c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856672"
---
# <a name="fileurlthreatsubmission-resource-type"></a>fileUrlThreatSubmission 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示使用文件 URL 提交时创建的文件威胁提交对象。 此 API 是保留的，当前不支持。

继承自 [fileThreatSubmission](../resources/security-filethreatsubmission.md)。

## <a name="properties"></a>属性
| 属性 | 类型   | Description                   |
|:---------|:-------|:------------------------------|
| fileUrl  | String | 它指定需要提交的文件的 URL。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileUrlThreatSubmission",
  "baseType": "microsoft.graph.security.fileThreatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileUrlThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "fileName": "String",
  "fileUrl": "String"
}
```

