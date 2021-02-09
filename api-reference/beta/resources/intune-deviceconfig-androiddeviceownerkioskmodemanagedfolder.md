---
title: androidDeviceOwnerKioskModeManagedFolder 资源类型
description: 一个文件夹，其中包含托管主屏幕上的应用页面和 Web 链接
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6b373729ffebb3fc7a08ee29e98f3471c8c27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162264"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a><span data-ttu-id="4f361-103">androidDeviceOwnerKioskModeManagedFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f361-103">androidDeviceOwnerKioskModeManagedFolder resource type</span></span>

<span data-ttu-id="4f361-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f361-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f361-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f361-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f361-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f361-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f361-107">一个文件夹，其中包含托管主屏幕上的应用页面和 Web 链接</span><span class="sxs-lookup"><span data-stu-id="4f361-107">A folder containing pages of apps and weblinks on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="4f361-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f361-108">Properties</span></span>
|<span data-ttu-id="4f361-109">属性</span><span class="sxs-lookup"><span data-stu-id="4f361-109">Property</span></span>|<span data-ttu-id="4f361-110">类型</span><span class="sxs-lookup"><span data-stu-id="4f361-110">Type</span></span>|<span data-ttu-id="4f361-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f361-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f361-112">folderName</span><span class="sxs-lookup"><span data-stu-id="4f361-112">folderName</span></span>|<span data-ttu-id="4f361-113">String</span><span class="sxs-lookup"><span data-stu-id="4f361-113">String</span></span>|<span data-ttu-id="4f361-114">文件夹的显示名称</span><span class="sxs-lookup"><span data-stu-id="4f361-114">Display name for the folder</span></span>|
|<span data-ttu-id="4f361-115">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f361-115">folderIdentifier</span></span>|<span data-ttu-id="4f361-116">String</span><span class="sxs-lookup"><span data-stu-id="4f361-116">String</span></span>|<span data-ttu-id="4f361-117">文件夹的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="4f361-117">Unique identifier for the folder</span></span>|
|<span data-ttu-id="4f361-118">items</span><span class="sxs-lookup"><span data-stu-id="4f361-118">items</span></span>|<span data-ttu-id="4f361-119">[androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f361-119">[androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md) collection</span></span>|<span data-ttu-id="4f361-120">要添加到托管文件夹的项目。</span><span class="sxs-lookup"><span data-stu-id="4f361-120">Items to be added to managed folder.</span></span> <span data-ttu-id="4f361-121">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4f361-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f361-122">关系</span><span class="sxs-lookup"><span data-stu-id="4f361-122">Relationships</span></span>
<span data-ttu-id="4f361-123">无</span><span class="sxs-lookup"><span data-stu-id="4f361-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f361-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f361-124">JSON Representation</span></span>
<span data-ttu-id="4f361-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f361-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```




