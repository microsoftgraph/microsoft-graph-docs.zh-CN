---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a2965a2ba1f30d19e4f755caa0d10676d110f41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730344"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="0a762-103">mobileAppInstallTimeSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a762-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="0a762-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a762-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a762-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a762-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a762-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a762-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a762-107">包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="0a762-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="0a762-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a762-108">Properties</span></span>
|<span data-ttu-id="0a762-109">属性</span><span class="sxs-lookup"><span data-stu-id="0a762-109">Property</span></span>|<span data-ttu-id="0a762-110">类型</span><span class="sxs-lookup"><span data-stu-id="0a762-110">Type</span></span>|<span data-ttu-id="0a762-111">说明</span><span class="sxs-lookup"><span data-stu-id="0a762-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a762-112">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="0a762-112">useLocalTime</span></span>|<span data-ttu-id="0a762-113">布尔</span><span class="sxs-lookup"><span data-stu-id="0a762-113">Boolean</span></span>|<span data-ttu-id="0a762-114">确定可用时间和截止时间时，是否应使用本地设备时间或 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0a762-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="0a762-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0a762-115">startDateTime</span></span>|<span data-ttu-id="0a762-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a762-116">DateTimeOffset</span></span>|<span data-ttu-id="0a762-117">应用程序可供安装的时间。</span><span class="sxs-lookup"><span data-stu-id="0a762-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="0a762-118">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="0a762-118">deadlineDateTime</span></span>|<span data-ttu-id="0a762-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a762-119">DateTimeOffset</span></span>|<span data-ttu-id="0a762-120">应安装应用程序的时间。</span><span class="sxs-lookup"><span data-stu-id="0a762-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a762-121">关系</span><span class="sxs-lookup"><span data-stu-id="0a762-121">Relationships</span></span>
<span data-ttu-id="0a762-122">无</span><span class="sxs-lookup"><span data-stu-id="0a762-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a762-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a762-123">JSON Representation</span></span>
<span data-ttu-id="0a762-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a762-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```





