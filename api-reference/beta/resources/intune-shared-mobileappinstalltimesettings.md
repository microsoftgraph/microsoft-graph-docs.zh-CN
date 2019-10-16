---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d99505990bb19789046521632441c4026a0ee404
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538712"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="c0eeb-103">mobileAppInstallTimeSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0eeb-103">mobileAppInstallTimeSettings resource type</span></span>

> <span data-ttu-id="c0eeb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0eeb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0eeb-106">包含用于确定何时向设备提供应用程序以及何时在设备上安装应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="c0eeb-107">属性</span><span class="sxs-lookup"><span data-stu-id="c0eeb-107">Properties</span></span>
|<span data-ttu-id="c0eeb-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0eeb-108">Property</span></span>|<span data-ttu-id="c0eeb-109">类型</span><span class="sxs-lookup"><span data-stu-id="c0eeb-109">Type</span></span>|<span data-ttu-id="c0eeb-110">说明</span><span class="sxs-lookup"><span data-stu-id="c0eeb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0eeb-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="c0eeb-111">useLocalTime</span></span>|<span data-ttu-id="c0eeb-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0eeb-112">Boolean</span></span>|<span data-ttu-id="c0eeb-113">确定可用时间和截止时间时，是否应使用本地设备时间或 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="c0eeb-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c0eeb-114">startDateTime</span></span>|<span data-ttu-id="c0eeb-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0eeb-115">DateTimeOffset</span></span>|<span data-ttu-id="c0eeb-116">应用程序可供安装的时间。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="c0eeb-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="c0eeb-117">deadlineDateTime</span></span>|<span data-ttu-id="c0eeb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0eeb-118">DateTimeOffset</span></span>|<span data-ttu-id="c0eeb-119">应安装应用程序的时间。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0eeb-120">关系</span><span class="sxs-lookup"><span data-stu-id="c0eeb-120">Relationships</span></span>
<span data-ttu-id="c0eeb-121">无</span><span class="sxs-lookup"><span data-stu-id="c0eeb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0eeb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0eeb-122">JSON Representation</span></span>
<span data-ttu-id="c0eeb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0eeb-123">Here is a JSON representation of the resource.</span></span>
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



