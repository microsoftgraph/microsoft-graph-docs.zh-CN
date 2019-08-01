---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 754f5ce902ca4cb5bb63be41f0e8094cc0738c26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037637"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="02dd0-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="02dd0-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="02dd0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02dd0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02dd0-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="02dd0-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="02dd0-106">属性</span><span class="sxs-lookup"><span data-stu-id="02dd0-106">Properties</span></span>
|<span data-ttu-id="02dd0-107">属性</span><span class="sxs-lookup"><span data-stu-id="02dd0-107">Property</span></span>|<span data-ttu-id="02dd0-108">类型</span><span class="sxs-lookup"><span data-stu-id="02dd0-108">Type</span></span>|<span data-ttu-id="02dd0-109">说明</span><span class="sxs-lookup"><span data-stu-id="02dd0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02dd0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="02dd0-110">displayName</span></span>|<span data-ttu-id="02dd0-111">String</span><span class="sxs-lookup"><span data-stu-id="02dd0-111">String</span></span>|<span data-ttu-id="02dd0-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="02dd0-112">Display name</span></span>|
|<span data-ttu-id="02dd0-113">资源</span><span class="sxs-lookup"><span data-stu-id="02dd0-113">resources</span></span>|<span data-ttu-id="02dd0-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="02dd0-114">String collection</span></span>|<span data-ttu-id="02dd0-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="02dd0-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="02dd0-116">关系</span><span class="sxs-lookup"><span data-stu-id="02dd0-116">Relationships</span></span>
<span data-ttu-id="02dd0-117">无</span><span class="sxs-lookup"><span data-stu-id="02dd0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02dd0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02dd0-118">JSON Representation</span></span>
<span data-ttu-id="02dd0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02dd0-119">Here is a JSON representation of the resource.</span></span>
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



