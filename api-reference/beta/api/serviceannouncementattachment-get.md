---
title: 获取 serviceAnnouncementAttachment
description: 读取 serviceAnnouncementAttachment 对象的属性和关系。
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 7af0443414740ea548c5e332d9df5230353689f4
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072799"
---
# <a name="get-serviceannouncementattachment"></a>获取 serviceAnnouncementAttachment
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) 对象的属性和关系。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|ServiceMessage.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|ServiceMessage.Read.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}/attachments/{serviceAnnouncementAttachmentId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-get-an-attachment-with-message-id"></a>示例 1：获取具有邮件 ID 的附件

以下请求返回 [serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) 资源。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC54091/attachments/30356a46-ffad-47e1-acf6-40a99b1538c1
```

#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#admin/serviceAnnouncement/messages('MC54091')/attachments/$entity",
    "contentType": "application/csv",
    "isInline": false,
    "lastModifiedDateTime": "2021-09-21T04:07:15.9720778Z",
    "name": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center.",
    "size": 44583,
    "id": "30356a46-ffad-47e1-acf6-40a99b1538c1"
  }
}
```

### <a name="example-2-return-a-file-stream-of-an-attachment-content-for-a-message"></a>示例 2：返回邮件的附件内容的文件流

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_serviceannouncementattachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC54091/attachments/30356a46-ffad-47e1-acf6-40a99b1538c1/content
```

#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "An attachment for a Data Privacy message regarding your organization is available within Message Center. The contents of this attachment can be accessed within Message Center by a Global Administrator or someone designated as a Message Center Privacy Reader. Please sign in to Admin Center to view the details of this message in the Microsoft 365 Message center."
}
```
