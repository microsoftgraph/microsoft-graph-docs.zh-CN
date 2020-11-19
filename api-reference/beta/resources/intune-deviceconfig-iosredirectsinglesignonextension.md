---
title: iosRedirectSingleSignOnExtension 资源类型
description: 表示 iOS 设备的重定向类型单一 Sign-On 扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40148b36984ae2239465410ed66d1427e1aed60a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280114"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="8d339-103">iosRedirectSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d339-103">iosRedirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="8d339-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d339-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d339-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d339-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d339-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d339-107">表示 iOS 设备的重定向类型单一 Sign-On 扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="8d339-107">Represents a Redirect-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="8d339-108">继承自 [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="8d339-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d339-109">属性</span><span class="sxs-lookup"><span data-stu-id="8d339-109">Properties</span></span>
|<span data-ttu-id="8d339-110">属性</span><span class="sxs-lookup"><span data-stu-id="8d339-110">Property</span></span>|<span data-ttu-id="8d339-111">类型</span><span class="sxs-lookup"><span data-stu-id="8d339-111">Type</span></span>|<span data-ttu-id="8d339-112">说明</span><span class="sxs-lookup"><span data-stu-id="8d339-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d339-113">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="8d339-113">extensionIdentifier</span></span>|<span data-ttu-id="8d339-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8d339-114">String</span></span>|<span data-ttu-id="8d339-115">获取或设置对指定 Url 执行 SSO 的应用扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="8d339-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="8d339-116">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="8d339-116">teamIdentifier</span></span>|<span data-ttu-id="8d339-117">字符串</span><span class="sxs-lookup"><span data-stu-id="8d339-117">String</span></span>|<span data-ttu-id="8d339-118">获取或设置为指定的 Url 执行 SSO 的应用程序扩展的团队 ID。</span><span class="sxs-lookup"><span data-stu-id="8d339-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="8d339-119">配置</span><span class="sxs-lookup"><span data-stu-id="8d339-119">configurations</span></span>|<span data-ttu-id="8d339-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d339-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="8d339-121">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="8d339-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="8d339-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8d339-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8d339-123">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="8d339-123">urlPrefixes</span></span>|<span data-ttu-id="8d339-124">String 集合</span><span class="sxs-lookup"><span data-stu-id="8d339-124">String collection</span></span>|<span data-ttu-id="8d339-125">标识提供程序的一个或多个 URL 前缀，代表其应用程序扩展执行单一登录。</span><span class="sxs-lookup"><span data-stu-id="8d339-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="8d339-126">Url 必须以 http://或 https://开头。</span><span class="sxs-lookup"><span data-stu-id="8d339-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="8d339-127">所有 URL 前缀对所有配置文件都必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="8d339-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d339-128">关系</span><span class="sxs-lookup"><span data-stu-id="8d339-128">Relationships</span></span>
<span data-ttu-id="8d339-129">无</span><span class="sxs-lookup"><span data-stu-id="8d339-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d339-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d339-130">JSON Representation</span></span>
<span data-ttu-id="8d339-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d339-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```




