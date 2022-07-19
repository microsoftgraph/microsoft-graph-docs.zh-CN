---
title: fileThreatSubmission 资源类型
description: 表示与文件相关的威胁提交。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c592e2f0b5a22cf564a790c6f7934ba766771cd
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856675"
---
# <a name="filethreatsubmission-resource-type"></a>fileThreatSubmission 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与文件相关的威胁提交。 它用于向Microsoft Defender for Office 365提交可疑的恶意软件电子邮件附件。 它还可用于提交不应被Microsoft Defender for Office 365阻止的误报案例，例如安全的电子邮件附件。

目前，文件威胁提交会路由到Microsoft Defender for Office 365。 将来，它可能会路由到Microsoft Defender for Endpoint。 这是文件威胁提交（无论其路由到何处）的统一接口。

这是一种抽象类型。 继承自 [threatSubmission](../resources/security-threatsubmission.md)。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 fileThreatSubmissions](../api/security-filethreatsubmission-list.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md) 集合|获取 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象及其属性的列表。|
|[创建 fileThreatSubmission](../api/security-filethreatsubmission-post-filethreats.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|创建新的 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象。|
|[获取 fileThreatSubmission](../api/security-filethreatsubmission-get.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|读取 [fileThreatSubmission](../resources/security-filethreatsubmission.md) 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性 | 类型   | Description                    |
|:---------|:-------|:-------------------------------|
| fileName | String | 它指定要提交的文件名。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileThreatSubmission",
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
  "fileName": "String"
}
```

