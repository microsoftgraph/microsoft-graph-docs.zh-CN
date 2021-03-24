---
title: userExperienceAnalyticsCloudManagementDevicesSummary 资源类型
description: 用户体验从任意位置云管理设备摘要工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0fb4e7d9a8ac5b2ab9c134d45c2e625a935b491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146758"
---
# <a name="userexperienceanalyticscloudmanagementdevicessummary-resource-type"></a><span data-ttu-id="369cd-103">userExperienceAnalyticsCloudManagementDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="369cd-103">userExperienceAnalyticsCloudManagementDevicesSummary resource type</span></span>

<span data-ttu-id="369cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="369cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="369cd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="369cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="369cd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="369cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="369cd-107">用户体验从任意位置云管理设备摘要工作。</span><span class="sxs-lookup"><span data-stu-id="369cd-107">The user experience work from anywhere Cloud management devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="369cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="369cd-108">Properties</span></span>
|<span data-ttu-id="369cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="369cd-109">Property</span></span>|<span data-ttu-id="369cd-110">类型</span><span class="sxs-lookup"><span data-stu-id="369cd-110">Type</span></span>|<span data-ttu-id="369cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="369cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="369cd-112">coManagedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="369cd-112">coManagedDeviceCount</span></span>|<span data-ttu-id="369cd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="369cd-113">Int32</span></span>|<span data-ttu-id="369cd-114">共同管理的设备的总数。</span><span class="sxs-lookup"><span data-stu-id="369cd-114">Total number of  co-managed devices.</span></span>|
|<span data-ttu-id="369cd-115">intuneDeviceCount</span><span class="sxs-lookup"><span data-stu-id="369cd-115">intuneDeviceCount</span></span>|<span data-ttu-id="369cd-116">Int32</span><span class="sxs-lookup"><span data-stu-id="369cd-116">Int32</span></span>|<span data-ttu-id="369cd-117">未注册 autopilot 的 intune 设备计数。</span><span class="sxs-lookup"><span data-stu-id="369cd-117">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="369cd-118">tenantAttachDeviceCount</span><span class="sxs-lookup"><span data-stu-id="369cd-118">tenantAttachDeviceCount</span></span>|<span data-ttu-id="369cd-119">Int32</span><span class="sxs-lookup"><span data-stu-id="369cd-119">Int32</span></span>|<span data-ttu-id="369cd-120">租户附加设备总数。</span><span class="sxs-lookup"><span data-stu-id="369cd-120">Total count of tenant attach devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="369cd-121">关系</span><span class="sxs-lookup"><span data-stu-id="369cd-121">Relationships</span></span>
<span data-ttu-id="369cd-122">无</span><span class="sxs-lookup"><span data-stu-id="369cd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="369cd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="369cd-123">JSON Representation</span></span>
<span data-ttu-id="369cd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="369cd-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
  "coManagedDeviceCount": 1024,
  "intuneDeviceCount": 1024,
  "tenantAttachDeviceCount": 1024
}
```




