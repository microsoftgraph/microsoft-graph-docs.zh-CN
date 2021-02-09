---
title: androidDeviceOwnerKioskModeManagedFolderReference 资源类型
description: 对托管主屏幕上包含应用和 Web 链接的文件夹的引用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f454abc8edb54e1ee2ed2e9a6984e8e9e39e29d2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162263"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a><span data-ttu-id="bc026-103">androidDeviceOwnerKioskModeManagedFolderReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc026-103">androidDeviceOwnerKioskModeManagedFolderReference resource type</span></span>

<span data-ttu-id="bc026-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc026-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc026-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc026-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc026-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc026-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc026-107">对托管主屏幕上包含应用和 Web 链接的文件夹的引用</span><span class="sxs-lookup"><span data-stu-id="bc026-107">A reference to folder containing apps and weblinks on the Managed Home Screen</span></span>


<span data-ttu-id="bc026-108">继承自 [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc026-108">Inherits from [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc026-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc026-109">Properties</span></span>
|<span data-ttu-id="bc026-110">属性</span><span class="sxs-lookup"><span data-stu-id="bc026-110">Property</span></span>|<span data-ttu-id="bc026-111">类型</span><span class="sxs-lookup"><span data-stu-id="bc026-111">Type</span></span>|<span data-ttu-id="bc026-112">说明</span><span class="sxs-lookup"><span data-stu-id="bc026-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc026-113">folderName</span><span class="sxs-lookup"><span data-stu-id="bc026-113">folderName</span></span>|<span data-ttu-id="bc026-114">String</span><span class="sxs-lookup"><span data-stu-id="bc026-114">String</span></span>|<span data-ttu-id="bc026-115">文件夹的名称</span><span class="sxs-lookup"><span data-stu-id="bc026-115">Name of the folder</span></span>|
|<span data-ttu-id="bc026-116">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc026-116">folderIdentifier</span></span>|<span data-ttu-id="bc026-117">String</span><span class="sxs-lookup"><span data-stu-id="bc026-117">String</span></span>|<span data-ttu-id="bc026-118">文件夹的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bc026-118">Unique identifier for the folder</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc026-119">关系</span><span class="sxs-lookup"><span data-stu-id="bc026-119">Relationships</span></span>
<span data-ttu-id="bc026-120">无</span><span class="sxs-lookup"><span data-stu-id="bc026-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc026-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc026-121">JSON Representation</span></span>
<span data-ttu-id="bc026-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc026-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```




