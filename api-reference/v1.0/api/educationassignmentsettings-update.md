---
title: 更新 educationAssignmentSettings
description: 更新 educationAssignmentSettings 对象的属性。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11802b1b2fadfc717a123db31ad91436183442ed
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912357"
---
# <a name="update-educationassignmentsettings"></a>更新 educationAssignmentSettings
命名空间：microsoft.graph

更新 [educationAssignmentSettings 对象](../resources/educationassignmentsettings.md) 的属性。 只有教师可以更新这些设置。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象的 JSON 表示形式。

下表显示更新 [educationAssignmentSettings 时所需的属性](../resources/educationassignmentsettings.md)。

|属性|类型|说明|
|:---|:---|:---|
|submissionAnimationDisabled|Boolean|指示是否显示打开的庆祝动画。 的值 `true` 指示不会显示动画。 默认值为 `false`。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```

### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "submissionAnimationDisabled": true
}
```

