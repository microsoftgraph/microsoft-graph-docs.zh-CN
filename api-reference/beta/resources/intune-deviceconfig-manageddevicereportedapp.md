---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e1cd99974259835859cf8a2fc6a9f197c09d4d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166267"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="2249d-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="2249d-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="2249d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2249d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2249d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2249d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2249d-106">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="2249d-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="2249d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2249d-107">Properties</span></span>
|<span data-ttu-id="2249d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2249d-108">Property</span></span>|<span data-ttu-id="2249d-109">类型</span><span class="sxs-lookup"><span data-stu-id="2249d-109">Type</span></span>|<span data-ttu-id="2249d-110">说明</span><span class="sxs-lookup"><span data-stu-id="2249d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2249d-111">appId</span><span class="sxs-lookup"><span data-stu-id="2249d-111">appId</span></span>|<span data-ttu-id="2249d-112">String</span><span class="sxs-lookup"><span data-stu-id="2249d-112">String</span></span>|<span data-ttu-id="2249d-113">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="2249d-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="2249d-114">关系</span><span class="sxs-lookup"><span data-stu-id="2249d-114">Relationships</span></span>
<span data-ttu-id="2249d-115">无</span><span class="sxs-lookup"><span data-stu-id="2249d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2249d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2249d-116">JSON Representation</span></span>
<span data-ttu-id="2249d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2249d-117">Here is a JSON representation of the resource.</span></span>
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




