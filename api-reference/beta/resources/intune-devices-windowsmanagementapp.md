---
title: windowsManagementApp 资源类型
description: Windows 管理应用程序实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 395148d4c870193d75f418d7dc30d2b2241bad01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913497"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="06683-103">windowsManagementApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="06683-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="06683-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06683-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06683-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06683-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06683-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06683-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06683-107">Windows 管理应用程序实体。</span><span class="sxs-lookup"><span data-stu-id="06683-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="06683-108">方法</span><span class="sxs-lookup"><span data-stu-id="06683-108">Methods</span></span>
|<span data-ttu-id="06683-109">方法</span><span class="sxs-lookup"><span data-stu-id="06683-109">Method</span></span>|<span data-ttu-id="06683-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06683-110">Return Type</span></span>|<span data-ttu-id="06683-111">说明</span><span class="sxs-lookup"><span data-stu-id="06683-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06683-112">获取 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="06683-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="06683-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="06683-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="06683-114">读取属性和[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="06683-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="06683-115">更新 windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="06683-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="06683-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="06683-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="06683-117">更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06683-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06683-118">属性</span><span class="sxs-lookup"><span data-stu-id="06683-118">Properties</span></span>
|<span data-ttu-id="06683-119">属性</span><span class="sxs-lookup"><span data-stu-id="06683-119">Property</span></span>|<span data-ttu-id="06683-120">类型</span><span class="sxs-lookup"><span data-stu-id="06683-120">Type</span></span>|<span data-ttu-id="06683-121">说明</span><span class="sxs-lookup"><span data-stu-id="06683-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06683-122">id</span><span class="sxs-lookup"><span data-stu-id="06683-122">id</span></span>|<span data-ttu-id="06683-123">字符串</span><span class="sxs-lookup"><span data-stu-id="06683-123">String</span></span>|<span data-ttu-id="06683-124">Windows 管理应用程序的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="06683-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="06683-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="06683-125">availableVersion</span></span>|<span data-ttu-id="06683-126">字符串</span><span class="sxs-lookup"><span data-stu-id="06683-126">String</span></span>|<span data-ttu-id="06683-127">Windows 管理应用程序可用版本。</span><span class="sxs-lookup"><span data-stu-id="06683-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06683-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="06683-128">Relationships</span></span>
|<span data-ttu-id="06683-129">关系</span><span class="sxs-lookup"><span data-stu-id="06683-129">Relationship</span></span>|<span data-ttu-id="06683-130">类型</span><span class="sxs-lookup"><span data-stu-id="06683-130">Type</span></span>|<span data-ttu-id="06683-131">说明</span><span class="sxs-lookup"><span data-stu-id="06683-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06683-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="06683-132">healthSummary</span></span>|[<span data-ttu-id="06683-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="06683-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="06683-134">运行状况摘要 Windows 管理应用程序。</span><span class="sxs-lookup"><span data-stu-id="06683-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="06683-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="06683-135">healthStates</span></span>|<span data-ttu-id="06683-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合</span><span class="sxs-lookup"><span data-stu-id="06683-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="06683-137">安装 Windows 管理应用程序的运行状况状态的列表。</span><span class="sxs-lookup"><span data-stu-id="06683-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06683-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06683-138">JSON Representation</span></span>
<span data-ttu-id="06683-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06683-139">Here is a JSON representation of the resource.</span></span>
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





