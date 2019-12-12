---
title: redirectSingleSignOnExtension 资源类型
description: 表示 Apple 单一登录扩展。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a408d9cfd364f222ad87fd3796d7037ed51ab76a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955523"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="248f3-103">redirectSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="248f3-103">redirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="248f3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="248f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="248f3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="248f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="248f3-106">表示 Apple 单一登录扩展。</span><span class="sxs-lookup"><span data-stu-id="248f3-106">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="248f3-107">继承自[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="248f3-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="248f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="248f3-108">Properties</span></span>
|<span data-ttu-id="248f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="248f3-109">Property</span></span>|<span data-ttu-id="248f3-110">类型</span><span class="sxs-lookup"><span data-stu-id="248f3-110">Type</span></span>|<span data-ttu-id="248f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="248f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248f3-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="248f3-112">extensionIdentifier</span></span>|<span data-ttu-id="248f3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="248f3-113">String</span></span>|<span data-ttu-id="248f3-114">获取或设置对指定 Url 执行 SSO 的应用扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="248f3-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="248f3-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="248f3-115">teamIdentifier</span></span>|<span data-ttu-id="248f3-116">字符串</span><span class="sxs-lookup"><span data-stu-id="248f3-116">String</span></span>|<span data-ttu-id="248f3-117">获取或设置为指定的 Url 执行 SSO 的应用程序扩展的团队 ID。</span><span class="sxs-lookup"><span data-stu-id="248f3-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="248f3-118">配置</span><span class="sxs-lookup"><span data-stu-id="248f3-118">configurations</span></span>|<span data-ttu-id="248f3-119">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="248f3-119">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="248f3-120">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="248f3-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="248f3-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="248f3-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="248f3-122">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="248f3-122">urlPrefixes</span></span>|<span data-ttu-id="248f3-123">String collection</span><span class="sxs-lookup"><span data-stu-id="248f3-123">String collection</span></span>|<span data-ttu-id="248f3-124">标识提供程序的一个或多个 URL 前缀，代表其应用程序扩展执行单一登录。</span><span class="sxs-lookup"><span data-stu-id="248f3-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="248f3-125">Url 必须以 http://或 https://开头。</span><span class="sxs-lookup"><span data-stu-id="248f3-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="248f3-126">所有 URL 前缀对所有配置文件都必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="248f3-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="248f3-127">关系</span><span class="sxs-lookup"><span data-stu-id="248f3-127">Relationships</span></span>
<span data-ttu-id="248f3-128">无</span><span class="sxs-lookup"><span data-stu-id="248f3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="248f3-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="248f3-129">JSON Representation</span></span>
<span data-ttu-id="248f3-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="248f3-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.redirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.redirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



