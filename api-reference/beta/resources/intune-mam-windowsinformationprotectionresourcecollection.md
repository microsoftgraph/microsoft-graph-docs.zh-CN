---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99f8eed566c9fc2744e72e2a854acd527ae673bd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029916"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="44bb1-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="44bb1-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="44bb1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44bb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44bb1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44bb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44bb1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44bb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44bb1-107">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="44bb1-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="44bb1-108">属性</span><span class="sxs-lookup"><span data-stu-id="44bb1-108">Properties</span></span>
|<span data-ttu-id="44bb1-109">属性</span><span class="sxs-lookup"><span data-stu-id="44bb1-109">Property</span></span>|<span data-ttu-id="44bb1-110">类型</span><span class="sxs-lookup"><span data-stu-id="44bb1-110">Type</span></span>|<span data-ttu-id="44bb1-111">说明</span><span class="sxs-lookup"><span data-stu-id="44bb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44bb1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="44bb1-112">displayName</span></span>|<span data-ttu-id="44bb1-113">String</span><span class="sxs-lookup"><span data-stu-id="44bb1-113">String</span></span>|<span data-ttu-id="44bb1-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="44bb1-114">Display name</span></span>|
|<span data-ttu-id="44bb1-115">资源</span><span class="sxs-lookup"><span data-stu-id="44bb1-115">resources</span></span>|<span data-ttu-id="44bb1-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="44bb1-116">String collection</span></span>|<span data-ttu-id="44bb1-117">资源集合</span><span class="sxs-lookup"><span data-stu-id="44bb1-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="44bb1-118">关系</span><span class="sxs-lookup"><span data-stu-id="44bb1-118">Relationships</span></span>
<span data-ttu-id="44bb1-119">无</span><span class="sxs-lookup"><span data-stu-id="44bb1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44bb1-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44bb1-120">JSON Representation</span></span>
<span data-ttu-id="44bb1-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44bb1-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```






