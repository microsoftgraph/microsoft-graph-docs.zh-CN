---
title: driveItem： extractSensitivityLabels
description: 提取分配给驱动器项的一个或多个敏感度标签。
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f1e97e0be8cea61fa76b225159e22ad319c042d1
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917849"
---
# <a name="driveitem-extractsensitivitylabels"></a>driveItem： extractSensitivityLabels
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提取分配给驱动器项的一个或多个敏感度标签，并使用分配的标签的最新详细信息更新驱动器项的元数据。 如果无法提取文件的敏感度标签，则会引发提取错误，并显示适用的错误代码和消息。

> **注意**：此 API 仅适用于受支持的文件扩展名。 调用后，此 API 首先从数据库中检索文件的敏感度标签元数据，然后检查敏感度标签详细信息是否在文件内容方面是最新的。 如果是，则返回数据库中检索到的值。 如果没有，则从文件的内容流中提取敏感度标签，在数据库中更新相应的元数据，并返回新提取的值。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）                                                             |
|:--------------------------------------|:--------------------------------------------------------------------------------------------------------|
|委派（工作或学校帐户）     | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All   |
|委派（个人 Microsoft 帐户） | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All                                        |
|应用程序                            | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All                                |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/extractSensitivityLabels
POST /drives/{drive-id}/root:/{item-path}/extractSensitivityLabels
POST /groups/{group-id}/drive/items/{item-id}/extractSensitivityLabels
POST /groups/{group-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /me/drive/items/{item-id}/extractSensitivityLabels
POST /me/drive/root:/{item-path}/extractSensitivityLabels
POST /sites/{site-id}/drive/items/{item-id}/extractSensitivityLabels
POST /sites/{site-id}/drive/root:/{item-path}/extractSensitivityLabels
POST /users/{user-id}/drive/items/{item-id}/extractSensitivityLabels
POST /users/{user-id}/drive/root:/{item-path}/extractSensitivityLabels
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作将在响应正文中返回 `200 OK` 响应代码和 [extractSensitivityLabelsResult](../resources/extractsensitivitylabelsresult.md) 对象。

除了适用于 Microsoft Graph 的常规错误外，此 API 还返回`423 Locked`响应代码，该代码指示正在访问的文件已锁定。 在这种情况下，响应对象的 **代码** 属性指示阻止敏感度标签提取的错误类型。
下面是错误类型的可能值。

| 值                       | 说明                                                                                                         |
|:----------------------------|:--------------------------------------------------------------------------------------------------------------------|
| fileDoubleKeyEncrypted      | 指示通过双键加密保护文件;因此，无法打开它来提取敏感度标签。             |
| fileDecryptionNotSupported  | 指示加密文件具有特定属性，不允许SharePoint打开这些文件以提取敏感度标签。    |
| fileDecryptionDeferred      | 指示正在处理文件以进行解密;因此，无法打开它来提取敏感度标签。      |
| unknownFutureValue          | 可变枚举 sentinel 值。 请勿使用。                                                                   |

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- { "blockType": "request", "name": "extract-sensitivitylabels", "tags": "service.graph" } -->
``` http
POST https://graph.microsoft.com/beta/drive/root/items/016GVDAP3RCQS5VBQHORFIVU2ZMOSBL25U/extractSensitivityLabels
```


### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extractSensitivityLabelsResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.extractSensitivityLabelsResult",
    "labels": [
      {
        "sensitivityLabelId": "5feba255-812e-446a-ac59-a7044ef827b5",
        "assignmentMethod": "standard",
        "tenantId": "fed495cb-8c27-41ea-8749-00b0a084bc3d"
      },
      {
        "sensitivityLabelId": "fa781fdf-68c8-43ec-ae08-c4813deb2144",
        "assignmentMethod": "standard",
        "tenantId": "277601b1-6094-456c-a358-95bfc99539d7"
      },
      {
        "sensitivityLabelId": "3937098d-df0c-4c8d-8f66-5876b57b75ba",
        "assignmentMethod": "standard",
        "tenantId": "f2477f30-c8a2-422d-8995-6f056b494655"
      }
    ]
  }
}
```

