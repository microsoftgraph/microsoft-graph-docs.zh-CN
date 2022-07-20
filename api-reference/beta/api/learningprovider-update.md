---
title: 更新 learningProvider
description: 更新 learningProvider 对象的属性。
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: ac9ced68d3e3bad6ac794a6641bd98997ceb7633
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883299"
---
# <a name="update-learningprovider"></a>更新 learningProvider
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [learningProvider](../resources/learningprovider.md) 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|LearningProvider.ReadWrite|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /employeeExperience/learningProviders/{learningProviderId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|displayName|String|Viva Learning中显示的显示名称。 必需。|
|isEnabled|Boolean|提供程序的状态。 可选。|
|loginWebUrl|String|用于访问提供程序课程的身份验证 URL。 可选。|
|longLogoWebUrlForDarkTheme|String|深色模式的长徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|longLogoWebUrlForLightTheme|String|光模式的长徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|squareLogoWebUrlForDarkTheme|String|深色模式的方形徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|squareLogoWebUrlForLightTheme|String|光模式的方形徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|


## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "update_learningprovider"
}
-->
``` http
PATCH /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": false,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```


### <a name="response"></a>响应
下面展示了示例响应。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

