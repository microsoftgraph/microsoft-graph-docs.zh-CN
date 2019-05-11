---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76317a14d05ad1e4a949485f2ae63e00b1e91b81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944941"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="4e3bf-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e3bf-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="4e3bf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e3bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e3bf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e3bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3bf-106">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="4e3bf-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="4e3bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e3bf-107">Properties</span></span>
|<span data-ttu-id="4e3bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e3bf-108">Property</span></span>|<span data-ttu-id="4e3bf-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e3bf-109">Type</span></span>|<span data-ttu-id="4e3bf-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e3bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3bf-111">appId</span><span class="sxs-lookup"><span data-stu-id="4e3bf-111">appId</span></span>|<span data-ttu-id="4e3bf-112">String</span><span class="sxs-lookup"><span data-stu-id="4e3bf-112">String</span></span>|<span data-ttu-id="4e3bf-113">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="4e3bf-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e3bf-114">关系</span><span class="sxs-lookup"><span data-stu-id="4e3bf-114">Relationships</span></span>
<span data-ttu-id="4e3bf-115">无</span><span class="sxs-lookup"><span data-stu-id="4e3bf-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e3bf-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e3bf-116">JSON Representation</span></span>
<span data-ttu-id="4e3bf-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e3bf-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




