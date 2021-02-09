---
title: androidDeviceOwnerKioskModeApp 资源类型
description: Android 设备所有者托管主屏幕上的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6adb416c8fd20406c295e56a5d15177e625c30
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160556"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a><span data-ttu-id="e9081-103">androidDeviceOwnerKioskModeApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9081-103">androidDeviceOwnerKioskModeApp resource type</span></span>

<span data-ttu-id="e9081-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9081-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9081-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9081-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9081-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9081-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9081-107">Android 设备所有者托管主屏幕上的应用程序</span><span class="sxs-lookup"><span data-stu-id="e9081-107">An application on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="e9081-108">继承自 [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="e9081-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9081-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9081-109">Properties</span></span>
|<span data-ttu-id="e9081-110">属性</span><span class="sxs-lookup"><span data-stu-id="e9081-110">Property</span></span>|<span data-ttu-id="e9081-111">类型</span><span class="sxs-lookup"><span data-stu-id="e9081-111">Type</span></span>|<span data-ttu-id="e9081-112">说明</span><span class="sxs-lookup"><span data-stu-id="e9081-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9081-113">package</span><span class="sxs-lookup"><span data-stu-id="e9081-113">package</span></span>|<span data-ttu-id="e9081-114">String</span><span class="sxs-lookup"><span data-stu-id="e9081-114">String</span></span>|<span data-ttu-id="e9081-115">应用程序的程序包名称</span><span class="sxs-lookup"><span data-stu-id="e9081-115">Package name of application</span></span>|
|<span data-ttu-id="e9081-116">className</span><span class="sxs-lookup"><span data-stu-id="e9081-116">className</span></span>|<span data-ttu-id="e9081-117">String</span><span class="sxs-lookup"><span data-stu-id="e9081-117">String</span></span>|<span data-ttu-id="e9081-118">应用程序的类名</span><span class="sxs-lookup"><span data-stu-id="e9081-118">Class name of application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9081-119">关系</span><span class="sxs-lookup"><span data-stu-id="e9081-119">Relationships</span></span>
<span data-ttu-id="e9081-120">无</span><span class="sxs-lookup"><span data-stu-id="e9081-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9081-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9081-121">JSON Representation</span></span>
<span data-ttu-id="e9081-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9081-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```




