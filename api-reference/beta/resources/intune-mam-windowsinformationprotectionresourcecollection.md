---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5500f2bec507ae1f941d06e9cb7c22c94b301ba7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691230"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="6b4bf-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b4bf-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="6b4bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b4bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b4bf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b4bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b4bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b4bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b4bf-107">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="6b4bf-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6b4bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b4bf-108">Properties</span></span>
|<span data-ttu-id="6b4bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b4bf-109">Property</span></span>|<span data-ttu-id="6b4bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b4bf-110">Type</span></span>|<span data-ttu-id="6b4bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b4bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b4bf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6b4bf-112">displayName</span></span>|<span data-ttu-id="6b4bf-113">String</span><span class="sxs-lookup"><span data-stu-id="6b4bf-113">String</span></span>|<span data-ttu-id="6b4bf-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="6b4bf-114">Display name</span></span>|
|<span data-ttu-id="6b4bf-115">资源</span><span class="sxs-lookup"><span data-stu-id="6b4bf-115">resources</span></span>|<span data-ttu-id="6b4bf-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="6b4bf-116">String collection</span></span>|<span data-ttu-id="6b4bf-117">资源集合</span><span class="sxs-lookup"><span data-stu-id="6b4bf-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b4bf-118">关系</span><span class="sxs-lookup"><span data-stu-id="6b4bf-118">Relationships</span></span>
<span data-ttu-id="6b4bf-119">无</span><span class="sxs-lookup"><span data-stu-id="6b4bf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b4bf-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b4bf-120">JSON Representation</span></span>
<span data-ttu-id="6b4bf-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b4bf-121">Here is a JSON representation of the resource.</span></span>
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





