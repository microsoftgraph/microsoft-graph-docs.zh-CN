---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office配置 AAD 组分配目标。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d951db7a71474cc405f4b7f97419f1a06dd502d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666862"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="0f7ff-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f7ff-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="0f7ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f7ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f7ff-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f7ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f7ff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f7ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f7ff-107">Office配置 AAD 组分配目标。</span><span class="sxs-lookup"><span data-stu-id="0f7ff-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="0f7ff-108">继承自 [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0f7ff-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f7ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f7ff-109">Properties</span></span>
|<span data-ttu-id="0f7ff-110">属性</span><span class="sxs-lookup"><span data-stu-id="0f7ff-110">Property</span></span>|<span data-ttu-id="0f7ff-111">类型</span><span class="sxs-lookup"><span data-stu-id="0f7ff-111">Type</span></span>|<span data-ttu-id="0f7ff-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f7ff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f7ff-113">groupId</span><span class="sxs-lookup"><span data-stu-id="0f7ff-113">groupId</span></span>|<span data-ttu-id="0f7ff-114">String</span><span class="sxs-lookup"><span data-stu-id="0f7ff-114">String</span></span>|<span data-ttu-id="0f7ff-115">面向设备配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="0f7ff-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f7ff-116">关系</span><span class="sxs-lookup"><span data-stu-id="0f7ff-116">Relationships</span></span>
<span data-ttu-id="0f7ff-117">无</span><span class="sxs-lookup"><span data-stu-id="0f7ff-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f7ff-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f7ff-118">JSON Representation</span></span>
<span data-ttu-id="0f7ff-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f7ff-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```




