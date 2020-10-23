---
title: androidManagedStoreAppTrack 资源类型
description: 包含适用于 Android 托管存储应用的跟踪信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab4009dfb8fc6cfd40ae49529e07a6a6932d7c4d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690271"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="b94ce-103">androidManagedStoreAppTrack 资源类型</span><span class="sxs-lookup"><span data-stu-id="b94ce-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="b94ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b94ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b94ce-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b94ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b94ce-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b94ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b94ce-107">包含适用于 Android 托管存储应用的跟踪信息。</span><span class="sxs-lookup"><span data-stu-id="b94ce-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="b94ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="b94ce-108">Properties</span></span>
|<span data-ttu-id="b94ce-109">属性</span><span class="sxs-lookup"><span data-stu-id="b94ce-109">Property</span></span>|<span data-ttu-id="b94ce-110">类型</span><span class="sxs-lookup"><span data-stu-id="b94ce-110">Type</span></span>|<span data-ttu-id="b94ce-111">说明</span><span class="sxs-lookup"><span data-stu-id="b94ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b94ce-112">trackId</span><span class="sxs-lookup"><span data-stu-id="b94ce-112">trackId</span></span>|<span data-ttu-id="b94ce-113">String</span><span class="sxs-lookup"><span data-stu-id="b94ce-113">String</span></span>|<span data-ttu-id="b94ce-114">唯一的曲目标识符。</span><span class="sxs-lookup"><span data-stu-id="b94ce-114">Unique track identifier.</span></span>|
|<span data-ttu-id="b94ce-115">trackAlias</span><span class="sxs-lookup"><span data-stu-id="b94ce-115">trackAlias</span></span>|<span data-ttu-id="b94ce-116">String</span><span class="sxs-lookup"><span data-stu-id="b94ce-116">String</span></span>|<span data-ttu-id="b94ce-117">跟踪的友好名称。</span><span class="sxs-lookup"><span data-stu-id="b94ce-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b94ce-118">关系</span><span class="sxs-lookup"><span data-stu-id="b94ce-118">Relationships</span></span>
<span data-ttu-id="b94ce-119">无</span><span class="sxs-lookup"><span data-stu-id="b94ce-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b94ce-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b94ce-120">JSON Representation</span></span>
<span data-ttu-id="b94ce-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b94ce-121">Here is a JSON representation of the resource.</span></span>
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





