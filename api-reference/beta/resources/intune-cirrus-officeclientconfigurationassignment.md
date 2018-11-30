---
title: officeClientConfigurationAssignment 资源类型
description: Office 客户端配置工作分配。
ms.openlocfilehash: 7a2aeaace5fb929cddee16b4b43de8165509c7e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045299"
---
# <a name="officeclientconfigurationassignment-resource-type"></a><span data-ttu-id="1c15f-103">officeClientConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c15f-103">officeClientConfigurationAssignment resource type</span></span>

> <span data-ttu-id="1c15f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c15f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c15f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c15f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c15f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c15f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c15f-107">Office 客户端配置工作分配。</span><span class="sxs-lookup"><span data-stu-id="1c15f-107">Office Client Configuration Assignment.</span></span>
## <a name="methods"></a><span data-ttu-id="1c15f-108">方法</span><span class="sxs-lookup"><span data-stu-id="1c15f-108">Methods</span></span>
|<span data-ttu-id="1c15f-109">方法</span><span class="sxs-lookup"><span data-stu-id="1c15f-109">Method</span></span>|<span data-ttu-id="1c15f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c15f-110">Return Type</span></span>|<span data-ttu-id="1c15f-111">说明</span><span class="sxs-lookup"><span data-stu-id="1c15f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c15f-112">列表 officeClientConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="1c15f-112">List officeClientConfigurationAssignments</span></span>](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|<span data-ttu-id="1c15f-113">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c15f-113">[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1c15f-114">列出属性和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1c15f-114">List properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="1c15f-115">获取 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-115">Get officeClientConfigurationAssignment</span></span>](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[<span data-ttu-id="1c15f-116">officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-116">officeClientConfigurationAssignment</span></span>](../resources/intune-cirrus-officeclientconfigurationassignment.md)|<span data-ttu-id="1c15f-117">读取属性和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="1c15f-117">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1c15f-118">创建 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-118">Create officeClientConfigurationAssignment</span></span>](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[<span data-ttu-id="1c15f-119">officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-119">officeClientConfigurationAssignment</span></span>](../resources/intune-cirrus-officeclientconfigurationassignment.md)|<span data-ttu-id="1c15f-120">创建新的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c15f-120">Create a new [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1c15f-121">删除 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-121">Delete officeClientConfigurationAssignment</span></span>](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|<span data-ttu-id="1c15f-122">无</span><span class="sxs-lookup"><span data-stu-id="1c15f-122">None</span></span>|<span data-ttu-id="1c15f-123">删除[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="1c15f-123">Deletes a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="1c15f-124">更新 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-124">Update officeClientConfigurationAssignment</span></span>](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[<span data-ttu-id="1c15f-125">officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c15f-125">officeClientConfigurationAssignment</span></span>](../resources/intune-cirrus-officeclientconfigurationassignment.md)|<span data-ttu-id="1c15f-126">更新[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1c15f-126">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c15f-127">属性</span><span class="sxs-lookup"><span data-stu-id="1c15f-127">Properties</span></span>
|<span data-ttu-id="1c15f-128">属性</span><span class="sxs-lookup"><span data-stu-id="1c15f-128">Property</span></span>|<span data-ttu-id="1c15f-129">类型</span><span class="sxs-lookup"><span data-stu-id="1c15f-129">Type</span></span>|<span data-ttu-id="1c15f-130">说明</span><span class="sxs-lookup"><span data-stu-id="1c15f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c15f-131">id</span><span class="sxs-lookup"><span data-stu-id="1c15f-131">id</span></span>|<span data-ttu-id="1c15f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1c15f-132">String</span></span>|<span data-ttu-id="1c15f-133">OfficeConfigurationAssignment 的 id。</span><span class="sxs-lookup"><span data-stu-id="1c15f-133">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="1c15f-134">target</span><span class="sxs-lookup"><span data-stu-id="1c15f-134">target</span></span>|[<span data-ttu-id="1c15f-135">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1c15f-135">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="1c15f-136">目标工作分配定义的管理员。</span><span class="sxs-lookup"><span data-stu-id="1c15f-136">The target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c15f-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="1c15f-137">Relationships</span></span>
<span data-ttu-id="1c15f-138">无</span><span class="sxs-lookup"><span data-stu-id="1c15f-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c15f-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c15f-139">JSON Representation</span></span>
<span data-ttu-id="1c15f-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c15f-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



