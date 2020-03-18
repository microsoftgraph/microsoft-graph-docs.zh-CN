---
title: windowsManagementApp 资源类型
description: Windows 管理应用实体。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4dc0e11da5a669d42b13fc3ff81945726c18c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783611"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="3f25b-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f25b-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="3f25b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f25b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f25b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f25b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f25b-106">Windows 管理应用实体。</span><span class="sxs-lookup"><span data-stu-id="3f25b-106">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="3f25b-107">方法</span><span class="sxs-lookup"><span data-stu-id="3f25b-107">Methods</span></span>
|<span data-ttu-id="3f25b-108">方法</span><span class="sxs-lookup"><span data-stu-id="3f25b-108">Method</span></span>|<span data-ttu-id="3f25b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f25b-109">Return Type</span></span>|<span data-ttu-id="3f25b-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f25b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f25b-111">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3f25b-111">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="3f25b-112">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3f25b-112">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3f25b-113">读取[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f25b-113">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="3f25b-114">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3f25b-114">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="3f25b-115">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3f25b-115">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3f25b-116">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f25b-116">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f25b-117">属性</span><span class="sxs-lookup"><span data-stu-id="3f25b-117">Properties</span></span>
|<span data-ttu-id="3f25b-118">属性</span><span class="sxs-lookup"><span data-stu-id="3f25b-118">Property</span></span>|<span data-ttu-id="3f25b-119">类型</span><span class="sxs-lookup"><span data-stu-id="3f25b-119">Type</span></span>|<span data-ttu-id="3f25b-120">说明</span><span class="sxs-lookup"><span data-stu-id="3f25b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f25b-121">id</span><span class="sxs-lookup"><span data-stu-id="3f25b-121">id</span></span>|<span data-ttu-id="3f25b-122">String</span><span class="sxs-lookup"><span data-stu-id="3f25b-122">String</span></span>|<span data-ttu-id="3f25b-123">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="3f25b-123">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="3f25b-124">availableVersion</span><span class="sxs-lookup"><span data-stu-id="3f25b-124">availableVersion</span></span>|<span data-ttu-id="3f25b-125">String</span><span class="sxs-lookup"><span data-stu-id="3f25b-125">String</span></span>|<span data-ttu-id="3f25b-126">Windows 管理应用程序的可用版本。</span><span class="sxs-lookup"><span data-stu-id="3f25b-126">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f25b-127">关系</span><span class="sxs-lookup"><span data-stu-id="3f25b-127">Relationships</span></span>
|<span data-ttu-id="3f25b-128">关系</span><span class="sxs-lookup"><span data-stu-id="3f25b-128">Relationship</span></span>|<span data-ttu-id="3f25b-129">类型</span><span class="sxs-lookup"><span data-stu-id="3f25b-129">Type</span></span>|<span data-ttu-id="3f25b-130">说明</span><span class="sxs-lookup"><span data-stu-id="3f25b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f25b-131">healthStates</span><span class="sxs-lookup"><span data-stu-id="3f25b-131">healthStates</span></span>|<span data-ttu-id="3f25b-132">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f25b-132">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="3f25b-133">已安装的 Windows management 应用的运行状况状态列表。</span><span class="sxs-lookup"><span data-stu-id="3f25b-133">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f25b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f25b-134">JSON Representation</span></span>
<span data-ttu-id="3f25b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f25b-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```



