---
title: credentialSingleSignOnExtension 资源类型
description: 表示凭据类型的单一登录扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 51c003d84cb323a0fb049be52e46a7d5fce5112b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453469"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="35d29-103">credentialSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d29-103">credentialSingleSignOnExtension resource type</span></span>

<span data-ttu-id="35d29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35d29-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35d29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d29-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d29-107">表示凭据类型的单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="35d29-107">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="35d29-108">继承自[singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="35d29-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35d29-109">属性</span><span class="sxs-lookup"><span data-stu-id="35d29-109">Properties</span></span>
|<span data-ttu-id="35d29-110">属性</span><span class="sxs-lookup"><span data-stu-id="35d29-110">Property</span></span>|<span data-ttu-id="35d29-111">类型</span><span class="sxs-lookup"><span data-stu-id="35d29-111">Type</span></span>|<span data-ttu-id="35d29-112">说明</span><span class="sxs-lookup"><span data-stu-id="35d29-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d29-113">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="35d29-113">extensionIdentifier</span></span>|<span data-ttu-id="35d29-114">String</span><span class="sxs-lookup"><span data-stu-id="35d29-114">String</span></span>|<span data-ttu-id="35d29-115">获取或设置对指定 Url 执行 SSO 的应用扩展的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="35d29-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="35d29-116">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="35d29-116">teamIdentifier</span></span>|<span data-ttu-id="35d29-117">String</span><span class="sxs-lookup"><span data-stu-id="35d29-117">String</span></span>|<span data-ttu-id="35d29-118">获取或设置为指定的 Url 执行 SSO 的应用程序扩展的团队 ID。</span><span class="sxs-lookup"><span data-stu-id="35d29-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="35d29-119">域</span><span class="sxs-lookup"><span data-stu-id="35d29-119">domains</span></span>|<span data-ttu-id="35d29-120">String 集合</span><span class="sxs-lookup"><span data-stu-id="35d29-120">String collection</span></span>|<span data-ttu-id="35d29-121">获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。</span><span class="sxs-lookup"><span data-stu-id="35d29-121">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="35d29-122">型</span><span class="sxs-lookup"><span data-stu-id="35d29-122">realm</span></span>|<span data-ttu-id="35d29-123">String</span><span class="sxs-lookup"><span data-stu-id="35d29-123">String</span></span>|<span data-ttu-id="35d29-124">获取或设置此配置文件的区分大小写的领域名称。</span><span class="sxs-lookup"><span data-stu-id="35d29-124">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="35d29-125">配置</span><span class="sxs-lookup"><span data-stu-id="35d29-125">configurations</span></span>|<span data-ttu-id="35d29-126">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="35d29-126">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="35d29-127">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="35d29-127">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="35d29-128">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="35d29-128">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d29-129">关系</span><span class="sxs-lookup"><span data-stu-id="35d29-129">Relationships</span></span>
<span data-ttu-id="35d29-130">无</span><span class="sxs-lookup"><span data-stu-id="35d29-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d29-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d29-131">JSON Representation</span></span>
<span data-ttu-id="35d29-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d29-132">Here is a JSON representation of the resource.</span></span>
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



