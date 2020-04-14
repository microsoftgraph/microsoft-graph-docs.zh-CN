---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 858ce1825ab09709f412aeee978dc53a47a0d0af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455167"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="c10d1-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="c10d1-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="c10d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c10d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c10d1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c10d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c10d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c10d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c10d1-107">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="c10d1-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="c10d1-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c10d1-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c10d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="c10d1-109">Properties</span></span>
|<span data-ttu-id="c10d1-110">属性</span><span class="sxs-lookup"><span data-stu-id="c10d1-110">Property</span></span>|<span data-ttu-id="c10d1-111">类型</span><span class="sxs-lookup"><span data-stu-id="c10d1-111">Type</span></span>|<span data-ttu-id="c10d1-112">说明</span><span class="sxs-lookup"><span data-stu-id="c10d1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c10d1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c10d1-113">displayName</span></span>|<span data-ttu-id="c10d1-114">String</span><span class="sxs-lookup"><span data-stu-id="c10d1-114">String</span></span>|<span data-ttu-id="c10d1-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="c10d1-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c10d1-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="c10d1-116">bundleID</span></span>|<span data-ttu-id="c10d1-117">String</span><span class="sxs-lookup"><span data-stu-id="c10d1-117">String</span></span>|<span data-ttu-id="c10d1-118">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="c10d1-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c10d1-119">关系</span><span class="sxs-lookup"><span data-stu-id="c10d1-119">Relationships</span></span>
<span data-ttu-id="c10d1-120">无</span><span class="sxs-lookup"><span data-stu-id="c10d1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c10d1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c10d1-121">JSON Representation</span></span>
<span data-ttu-id="c10d1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c10d1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



