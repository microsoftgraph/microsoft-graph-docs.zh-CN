---
title: 创建 learningProvider
description: 创建新的 learningProvider 对象。
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: 40655e18f4fe22b3417f9ef2166538810ae36de4
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883284"
---
# <a name="create-learningprovider"></a>创建 learningProvider
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [learningProvider](../resources/learningprovider.md) 对象，并使用不同主题的指定显示名称和徽标向Viva Learning注册该对象。

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
POST /employeeExperience/learningProviders
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [learningProvider](../resources/learningprovider.md) 对象的 JSON 表示形式。

创建 **learningProvider** 时，可以指定以下属性。

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

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [learningProvider](../resources/learningprovider.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "create_learningprovider_from_"
}
-->
``` http
POST /employeeExperience/learningProviders 
Content-Type: application/json

{
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.learningProvider"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#learningProviders/$entity",
    "id": "ba9790ef-21d5-4c17-808c-acda55230253",
    "displayName": "Microsoft",
    "squareLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForDarkTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "squareLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "longLogoWebUrlForLightTheme": "https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png",
    "isEnabled": true,
    "loginWebUrl": "https://www.linkedin.com/learning-login/teams"
}
```

