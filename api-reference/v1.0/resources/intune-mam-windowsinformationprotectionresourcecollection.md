---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81b3a75533f70c57e31fe0f56770a281b66c61af
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366928"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="8029a-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="8029a-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="8029a-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8029a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8029a-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="8029a-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="8029a-106">属性</span><span class="sxs-lookup"><span data-stu-id="8029a-106">Properties</span></span>
|<span data-ttu-id="8029a-107">属性</span><span class="sxs-lookup"><span data-stu-id="8029a-107">Property</span></span>|<span data-ttu-id="8029a-108">类型</span><span class="sxs-lookup"><span data-stu-id="8029a-108">Type</span></span>|<span data-ttu-id="8029a-109">说明</span><span class="sxs-lookup"><span data-stu-id="8029a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8029a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8029a-110">displayName</span></span>|<span data-ttu-id="8029a-111">String</span><span class="sxs-lookup"><span data-stu-id="8029a-111">String</span></span>|<span data-ttu-id="8029a-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="8029a-112">Display name</span></span>|
|<span data-ttu-id="8029a-113">资源</span><span class="sxs-lookup"><span data-stu-id="8029a-113">resources</span></span>|<span data-ttu-id="8029a-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8029a-114">String collection</span></span>|<span data-ttu-id="8029a-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="8029a-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="8029a-116">关系</span><span class="sxs-lookup"><span data-stu-id="8029a-116">Relationships</span></span>
<span data-ttu-id="8029a-117">无</span><span class="sxs-lookup"><span data-stu-id="8029a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8029a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8029a-118">JSON Representation</span></span>
<span data-ttu-id="8029a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8029a-119">Here is a JSON representation of the resource.</span></span>
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




