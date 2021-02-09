---
title: androidDeviceOwnerKioskModeWeblink 资源类型
description: Android 设备所有者托管主屏幕上的 Web 链接
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 076e1fc6630856ff937bf85396c70e4461fda2b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162262"
---
# <a name="androiddeviceownerkioskmodeweblink-resource-type"></a><span data-ttu-id="8dc6d-103">androidDeviceOwnerKioskModeWeblink 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dc6d-103">androidDeviceOwnerKioskModeWeblink resource type</span></span>

<span data-ttu-id="8dc6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dc6d-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8dc6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dc6d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8dc6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dc6d-107">Android 设备所有者托管主屏幕上的 Web 链接</span><span class="sxs-lookup"><span data-stu-id="8dc6d-107">A weblink on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="8dc6d-108">继承自 [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="8dc6d-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8dc6d-109">属性</span><span class="sxs-lookup"><span data-stu-id="8dc6d-109">Properties</span></span>
|<span data-ttu-id="8dc6d-110">属性</span><span class="sxs-lookup"><span data-stu-id="8dc6d-110">Property</span></span>|<span data-ttu-id="8dc6d-111">类型</span><span class="sxs-lookup"><span data-stu-id="8dc6d-111">Type</span></span>|<span data-ttu-id="8dc6d-112">说明</span><span class="sxs-lookup"><span data-stu-id="8dc6d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc6d-113">label</span><span class="sxs-lookup"><span data-stu-id="8dc6d-113">label</span></span>|<span data-ttu-id="8dc6d-114">String</span><span class="sxs-lookup"><span data-stu-id="8dc6d-114">String</span></span>|<span data-ttu-id="8dc6d-115">Weblink 的显示名称</span><span class="sxs-lookup"><span data-stu-id="8dc6d-115">Display name for weblink</span></span>|
|<span data-ttu-id="8dc6d-116">link</span><span class="sxs-lookup"><span data-stu-id="8dc6d-116">link</span></span>|<span data-ttu-id="8dc6d-117">String</span><span class="sxs-lookup"><span data-stu-id="8dc6d-117">String</span></span>|<span data-ttu-id="8dc6d-118">Web 链接的链接</span><span class="sxs-lookup"><span data-stu-id="8dc6d-118">Link for weblink</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dc6d-119">关系</span><span class="sxs-lookup"><span data-stu-id="8dc6d-119">Relationships</span></span>
<span data-ttu-id="8dc6d-120">无</span><span class="sxs-lookup"><span data-stu-id="8dc6d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dc6d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dc6d-121">JSON Representation</span></span>
<span data-ttu-id="8dc6d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dc6d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeWeblink",
  "label": "String",
  "link": "String"
}
```




