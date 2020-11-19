---
title: deviceManagementConfigurationSettingOccurrence 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b8a93c75f011dba9816ee84a9ef8bf5cd05d275
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301596"
---
# <a name="devicemanagementconfigurationsettingoccurrence-resource-type"></a><span data-ttu-id="82eb9-103">deviceManagementConfigurationSettingOccurrence 资源类型</span><span class="sxs-lookup"><span data-stu-id="82eb9-103">deviceManagementConfigurationSettingOccurrence resource type</span></span>

<span data-ttu-id="82eb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82eb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82eb9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82eb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82eb9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82eb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82eb9-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="82eb9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="82eb9-108">属性</span><span class="sxs-lookup"><span data-stu-id="82eb9-108">Properties</span></span>
|<span data-ttu-id="82eb9-109">属性</span><span class="sxs-lookup"><span data-stu-id="82eb9-109">Property</span></span>|<span data-ttu-id="82eb9-110">类型</span><span class="sxs-lookup"><span data-stu-id="82eb9-110">Type</span></span>|<span data-ttu-id="82eb9-111">说明</span><span class="sxs-lookup"><span data-stu-id="82eb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82eb9-112">minDeviceOccurrence</span><span class="sxs-lookup"><span data-stu-id="82eb9-112">minDeviceOccurrence</span></span>|<span data-ttu-id="82eb9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="82eb9-113">Int32</span></span>|<span data-ttu-id="82eb9-114">可以在设备上设置 "最小时间" 设置。</span><span class="sxs-lookup"><span data-stu-id="82eb9-114">Minimum times setting can be set on device.</span></span> <span data-ttu-id="82eb9-115">MinDeviceOccurrence 为0表示设置是可选的</span><span class="sxs-lookup"><span data-stu-id="82eb9-115">A MinDeviceOccurrence of 0 means setting is optional</span></span>|
|<span data-ttu-id="82eb9-116">maxDeviceOccurrence</span><span class="sxs-lookup"><span data-stu-id="82eb9-116">maxDeviceOccurrence</span></span>|<span data-ttu-id="82eb9-117">Int32</span><span class="sxs-lookup"><span data-stu-id="82eb9-117">Int32</span></span>|<span data-ttu-id="82eb9-118">可以在设备上设置 "最大时间" 设置。</span><span class="sxs-lookup"><span data-stu-id="82eb9-118">Maximum times setting can be set on device.</span></span> |

## <a name="relationships"></a><span data-ttu-id="82eb9-119">关系</span><span class="sxs-lookup"><span data-stu-id="82eb9-119">Relationships</span></span>
<span data-ttu-id="82eb9-120">无</span><span class="sxs-lookup"><span data-stu-id="82eb9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82eb9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82eb9-121">JSON Representation</span></span>
<span data-ttu-id="82eb9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82eb9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingOccurrence",
  "minDeviceOccurrence": 1024,
  "maxDeviceOccurrence": 1024
}
```




