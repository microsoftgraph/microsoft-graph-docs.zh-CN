---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f48b7d02d40307eec25371a20e98b9efcf416a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086540"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="d4a4f-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4a4f-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="d4a4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4a4f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4a4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4a4f-106">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="d4a4f-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="d4a4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="d4a4f-107">Properties</span></span>
|<span data-ttu-id="d4a4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4a4f-108">Property</span></span>|<span data-ttu-id="d4a4f-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4a4f-109">Type</span></span>|<span data-ttu-id="d4a4f-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4a4f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a4f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d4a4f-111">displayName</span></span>|<span data-ttu-id="d4a4f-112">String</span><span class="sxs-lookup"><span data-stu-id="d4a4f-112">String</span></span>|<span data-ttu-id="d4a4f-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="d4a4f-113">Display name</span></span>|
|<span data-ttu-id="d4a4f-114">资源</span><span class="sxs-lookup"><span data-stu-id="d4a4f-114">resources</span></span>|<span data-ttu-id="d4a4f-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d4a4f-115">String collection</span></span>|<span data-ttu-id="d4a4f-116">资源集合</span><span class="sxs-lookup"><span data-stu-id="d4a4f-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4a4f-117">关系</span><span class="sxs-lookup"><span data-stu-id="d4a4f-117">Relationships</span></span>
<span data-ttu-id="d4a4f-118">无</span><span class="sxs-lookup"><span data-stu-id="d4a4f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4a4f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4a4f-119">JSON Representation</span></span>
<span data-ttu-id="d4a4f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4a4f-120">Here is a JSON representation of the resource.</span></span>
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









