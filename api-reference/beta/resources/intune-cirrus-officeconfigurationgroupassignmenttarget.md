---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组分配目标。
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b27ecf9284dcf4ddf52502dab524e5d77d346f1f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797302"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="0762b-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="0762b-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0762b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0762b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0762b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0762b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0762b-106">Office 客户端配置 AAD 组分配目标。</span><span class="sxs-lookup"><span data-stu-id="0762b-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="0762b-107">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="0762b-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0762b-108">属性</span><span class="sxs-lookup"><span data-stu-id="0762b-108">Properties</span></span>
|<span data-ttu-id="0762b-109">属性</span><span class="sxs-lookup"><span data-stu-id="0762b-109">Property</span></span>|<span data-ttu-id="0762b-110">类型</span><span class="sxs-lookup"><span data-stu-id="0762b-110">Type</span></span>|<span data-ttu-id="0762b-111">说明</span><span class="sxs-lookup"><span data-stu-id="0762b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0762b-112">groupId</span><span class="sxs-lookup"><span data-stu-id="0762b-112">groupId</span></span>|<span data-ttu-id="0762b-113">String</span><span class="sxs-lookup"><span data-stu-id="0762b-113">String</span></span>|<span data-ttu-id="0762b-114">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="0762b-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0762b-115">关系</span><span class="sxs-lookup"><span data-stu-id="0762b-115">Relationships</span></span>
<span data-ttu-id="0762b-116">无</span><span class="sxs-lookup"><span data-stu-id="0762b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0762b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0762b-117">JSON Representation</span></span>
<span data-ttu-id="0762b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0762b-118">Here is a JSON representation of the resource.</span></span>
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



