---
title: androidManagedStoreAppTrack 资源类型
description: 包含适用于 Android 托管存储应用的跟踪信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d979912a6e0d44708049164bee4f656a317e5ab4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284763"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="9c1ef-103">androidManagedStoreAppTrack 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c1ef-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="9c1ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c1ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c1ef-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c1ef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1ef-107">包含适用于 Android 托管存储应用的跟踪信息。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="9c1ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c1ef-108">Properties</span></span>
|<span data-ttu-id="9c1ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="9c1ef-109">Property</span></span>|<span data-ttu-id="9c1ef-110">类型</span><span class="sxs-lookup"><span data-stu-id="9c1ef-110">Type</span></span>|<span data-ttu-id="9c1ef-111">Description</span><span class="sxs-lookup"><span data-stu-id="9c1ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c1ef-112">trackId</span><span class="sxs-lookup"><span data-stu-id="9c1ef-112">trackId</span></span>|<span data-ttu-id="9c1ef-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9c1ef-113">String</span></span>|<span data-ttu-id="9c1ef-114">唯一的曲目标识符。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-114">Unique track identifier.</span></span>|
|<span data-ttu-id="9c1ef-115">trackAlias</span><span class="sxs-lookup"><span data-stu-id="9c1ef-115">trackAlias</span></span>|<span data-ttu-id="9c1ef-116">字符串</span><span class="sxs-lookup"><span data-stu-id="9c1ef-116">String</span></span>|<span data-ttu-id="9c1ef-117">跟踪的友好名称。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c1ef-118">关系</span><span class="sxs-lookup"><span data-stu-id="9c1ef-118">Relationships</span></span>
<span data-ttu-id="9c1ef-119">无</span><span class="sxs-lookup"><span data-stu-id="9c1ef-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c1ef-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c1ef-120">JSON Representation</span></span>
<span data-ttu-id="9c1ef-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c1ef-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```




