---
title: windowsManagementApp 资源类型
description: Windows 管理应用程序实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a3b311863422e25b7b1f2d0dda4780f152ba2c74
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393009"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="120ec-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="120ec-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="120ec-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="120ec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="120ec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="120ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="120ec-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="120ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120ec-107">Windows 管理应用程序实体。</span><span class="sxs-lookup"><span data-stu-id="120ec-107">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="120ec-108">方法</span><span class="sxs-lookup"><span data-stu-id="120ec-108">Methods</span></span>
|<span data-ttu-id="120ec-109">方法</span><span class="sxs-lookup"><span data-stu-id="120ec-109">Method</span></span>|<span data-ttu-id="120ec-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="120ec-110">Return Type</span></span>|<span data-ttu-id="120ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="120ec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="120ec-112">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="120ec-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="120ec-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="120ec-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="120ec-114">读取属性和[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="120ec-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="120ec-115">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="120ec-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="120ec-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="120ec-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="120ec-117">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="120ec-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="120ec-118">属性</span><span class="sxs-lookup"><span data-stu-id="120ec-118">Properties</span></span>
|<span data-ttu-id="120ec-119">属性</span><span class="sxs-lookup"><span data-stu-id="120ec-119">Property</span></span>|<span data-ttu-id="120ec-120">类型</span><span class="sxs-lookup"><span data-stu-id="120ec-120">Type</span></span>|<span data-ttu-id="120ec-121">说明</span><span class="sxs-lookup"><span data-stu-id="120ec-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120ec-122">id</span><span class="sxs-lookup"><span data-stu-id="120ec-122">id</span></span>|<span data-ttu-id="120ec-123">String</span><span class="sxs-lookup"><span data-stu-id="120ec-123">String</span></span>|<span data-ttu-id="120ec-124">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="120ec-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="120ec-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="120ec-125">availableVersion</span></span>|<span data-ttu-id="120ec-126">String</span><span class="sxs-lookup"><span data-stu-id="120ec-126">String</span></span>|<span data-ttu-id="120ec-127">Windows 管理应用程序可用版本。</span><span class="sxs-lookup"><span data-stu-id="120ec-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="120ec-128">关系</span><span class="sxs-lookup"><span data-stu-id="120ec-128">Relationships</span></span>
|<span data-ttu-id="120ec-129">关系</span><span class="sxs-lookup"><span data-stu-id="120ec-129">Relationship</span></span>|<span data-ttu-id="120ec-130">类型</span><span class="sxs-lookup"><span data-stu-id="120ec-130">Type</span></span>|<span data-ttu-id="120ec-131">说明</span><span class="sxs-lookup"><span data-stu-id="120ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120ec-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="120ec-132">healthSummary</span></span>|[<span data-ttu-id="120ec-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="120ec-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="120ec-134">运行状况摘要 Windows 管理应用程序。</span><span class="sxs-lookup"><span data-stu-id="120ec-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="120ec-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="120ec-135">healthStates</span></span>|<span data-ttu-id="120ec-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="120ec-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="120ec-137">安装 Windows 管理应用程序的运行状况状态的列表。</span><span class="sxs-lookup"><span data-stu-id="120ec-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="120ec-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="120ec-138">JSON Representation</span></span>
<span data-ttu-id="120ec-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="120ec-139">Here is a JSON representation of the resource.</span></span>
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




