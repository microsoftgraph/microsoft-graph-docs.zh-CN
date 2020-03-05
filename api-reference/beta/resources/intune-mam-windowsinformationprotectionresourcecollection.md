---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f656f66c38c372d592bfcbfed4b01455584436c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524235"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="dc4f4-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc4f4-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="dc4f4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dc4f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc4f4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc4f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc4f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4f4-107">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="dc4f4-107">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="dc4f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc4f4-108">Properties</span></span>
|<span data-ttu-id="dc4f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="dc4f4-109">Property</span></span>|<span data-ttu-id="dc4f4-110">类型</span><span class="sxs-lookup"><span data-stu-id="dc4f4-110">Type</span></span>|<span data-ttu-id="dc4f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc4f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4f4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="dc4f4-112">displayName</span></span>|<span data-ttu-id="dc4f4-113">String</span><span class="sxs-lookup"><span data-stu-id="dc4f4-113">String</span></span>|<span data-ttu-id="dc4f4-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="dc4f4-114">Display name</span></span>|
|<span data-ttu-id="dc4f4-115">资源</span><span class="sxs-lookup"><span data-stu-id="dc4f4-115">resources</span></span>|<span data-ttu-id="dc4f4-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="dc4f4-116">String collection</span></span>|<span data-ttu-id="dc4f4-117">资源集合</span><span class="sxs-lookup"><span data-stu-id="dc4f4-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc4f4-118">关系</span><span class="sxs-lookup"><span data-stu-id="dc4f4-118">Relationships</span></span>
<span data-ttu-id="dc4f4-119">无</span><span class="sxs-lookup"><span data-stu-id="dc4f4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc4f4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc4f4-120">JSON Representation</span></span>
<span data-ttu-id="dc4f4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc4f4-121">Here is a JSON representation of the resource.</span></span>
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



