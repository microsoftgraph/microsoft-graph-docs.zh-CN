---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 835a7f2f9a104b855a54de699dab83df744af5f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084182"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="492df-103">mobileAppInstallTimeSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="492df-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="492df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="492df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="492df-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="492df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="492df-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="492df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="492df-107">包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="492df-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="492df-108">属性</span><span class="sxs-lookup"><span data-stu-id="492df-108">Properties</span></span>
|<span data-ttu-id="492df-109">属性</span><span class="sxs-lookup"><span data-stu-id="492df-109">Property</span></span>|<span data-ttu-id="492df-110">类型</span><span class="sxs-lookup"><span data-stu-id="492df-110">Type</span></span>|<span data-ttu-id="492df-111">说明</span><span class="sxs-lookup"><span data-stu-id="492df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="492df-112">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="492df-112">useLocalTime</span></span>|<span data-ttu-id="492df-113">布尔</span><span class="sxs-lookup"><span data-stu-id="492df-113">Boolean</span></span>|<span data-ttu-id="492df-114">确定可用时间和截止时间时，是否应使用本地设备时间或 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="492df-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="492df-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="492df-115">startDateTime</span></span>|<span data-ttu-id="492df-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="492df-116">DateTimeOffset</span></span>|<span data-ttu-id="492df-117">应用程序可供安装的时间。</span><span class="sxs-lookup"><span data-stu-id="492df-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="492df-118">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="492df-118">deadlineDateTime</span></span>|<span data-ttu-id="492df-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="492df-119">DateTimeOffset</span></span>|<span data-ttu-id="492df-120">应安装应用程序的时间。</span><span class="sxs-lookup"><span data-stu-id="492df-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="492df-121">关系</span><span class="sxs-lookup"><span data-stu-id="492df-121">Relationships</span></span>
<span data-ttu-id="492df-122">无</span><span class="sxs-lookup"><span data-stu-id="492df-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="492df-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="492df-123">JSON Representation</span></span>
<span data-ttu-id="492df-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="492df-124">Here is a JSON representation of the resource.</span></span>
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






