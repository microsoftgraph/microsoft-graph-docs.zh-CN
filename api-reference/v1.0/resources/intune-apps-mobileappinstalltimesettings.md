---
title: mobileAppInstallTimeSettings 资源类型
description: 包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb768938ffa2e167f13a267451041b65f39011c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755117"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="53d0b-103">mobileAppInstallTimeSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="53d0b-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="53d0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53d0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53d0b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53d0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53d0b-106">包含用于确定何时向设备提供应用以及何时在设备上安装应用的属性。</span><span class="sxs-lookup"><span data-stu-id="53d0b-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="53d0b-107">属性</span><span class="sxs-lookup"><span data-stu-id="53d0b-107">Properties</span></span>
|<span data-ttu-id="53d0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="53d0b-108">Property</span></span>|<span data-ttu-id="53d0b-109">类型</span><span class="sxs-lookup"><span data-stu-id="53d0b-109">Type</span></span>|<span data-ttu-id="53d0b-110">说明</span><span class="sxs-lookup"><span data-stu-id="53d0b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53d0b-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="53d0b-111">useLocalTime</span></span>|<span data-ttu-id="53d0b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="53d0b-112">Boolean</span></span>|<span data-ttu-id="53d0b-113">确定可用和截止时间时，应该使用本地设备时间还是 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="53d0b-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="53d0b-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="53d0b-114">startDateTime</span></span>|<span data-ttu-id="53d0b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53d0b-115">DateTimeOffset</span></span>|<span data-ttu-id="53d0b-116">应用应可供安装的时间。</span><span class="sxs-lookup"><span data-stu-id="53d0b-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="53d0b-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="53d0b-117">deadlineDateTime</span></span>|<span data-ttu-id="53d0b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53d0b-118">DateTimeOffset</span></span>|<span data-ttu-id="53d0b-119">应安装应用的时间。</span><span class="sxs-lookup"><span data-stu-id="53d0b-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53d0b-120">关系</span><span class="sxs-lookup"><span data-stu-id="53d0b-120">Relationships</span></span>
<span data-ttu-id="53d0b-121">无</span><span class="sxs-lookup"><span data-stu-id="53d0b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53d0b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53d0b-122">JSON Representation</span></span>
<span data-ttu-id="53d0b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53d0b-123">Here is a JSON representation of the resource.</span></span>
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




