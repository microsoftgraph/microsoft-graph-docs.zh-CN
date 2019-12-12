---
title: credentialSingleSignOnExtension 资源类型
description: 表示凭据类型的单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9289416c33eaea89a24ffd01a1fb46026d1e7ef9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955699"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="13174-103">credentialSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="13174-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="13174-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13174-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13174-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13174-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13174-106">表示凭据类型的单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="13174-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="13174-107">继承自[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="13174-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13174-108">属性</span><span class="sxs-lookup"><span data-stu-id="13174-108">Properties</span></span>
|<span data-ttu-id="13174-109">属性</span><span class="sxs-lookup"><span data-stu-id="13174-109">Property</span></span>|<span data-ttu-id="13174-110">类型</span><span class="sxs-lookup"><span data-stu-id="13174-110">Type</span></span>|<span data-ttu-id="13174-111">说明</span><span class="sxs-lookup"><span data-stu-id="13174-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13174-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="13174-112">extensionIdentifier</span></span>|<span data-ttu-id="13174-113">字符串</span><span class="sxs-lookup"><span data-stu-id="13174-113">String</span></span>|<span data-ttu-id="13174-114">获取或设置对指定 Url 执行 SSO 的应用扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="13174-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="13174-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="13174-115">teamIdentifier</span></span>|<span data-ttu-id="13174-116">字符串</span><span class="sxs-lookup"><span data-stu-id="13174-116">String</span></span>|<span data-ttu-id="13174-117">获取或设置为指定的 Url 执行 SSO 的应用程序扩展的团队 ID。</span><span class="sxs-lookup"><span data-stu-id="13174-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="13174-118">域</span><span class="sxs-lookup"><span data-stu-id="13174-118">domains</span></span>|<span data-ttu-id="13174-119">String collection</span><span class="sxs-lookup"><span data-stu-id="13174-119">String collection</span></span>|<span data-ttu-id="13174-120">获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。</span><span class="sxs-lookup"><span data-stu-id="13174-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="13174-121">型</span><span class="sxs-lookup"><span data-stu-id="13174-121">realm</span></span>|<span data-ttu-id="13174-122">字符串</span><span class="sxs-lookup"><span data-stu-id="13174-122">String</span></span>|<span data-ttu-id="13174-123">获取或设置此配置文件的区分大小写的领域名称。</span><span class="sxs-lookup"><span data-stu-id="13174-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="13174-124">配置</span><span class="sxs-lookup"><span data-stu-id="13174-124">configurations</span></span>|<span data-ttu-id="13174-125">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="13174-125">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="13174-126">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="13174-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="13174-127">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="13174-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13174-128">关系</span><span class="sxs-lookup"><span data-stu-id="13174-128">Relationships</span></span>
<span data-ttu-id="13174-129">无</span><span class="sxs-lookup"><span data-stu-id="13174-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13174-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13174-130">JSON Representation</span></span>
<span data-ttu-id="13174-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13174-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



