---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: beeb1b8919e6e8caec0a055a5520c4a71c131e90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010183"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="7b095-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b095-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="7b095-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b095-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b095-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b095-107">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="7b095-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="7b095-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b095-108">Properties</span></span>
|<span data-ttu-id="7b095-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b095-109">Property</span></span>|<span data-ttu-id="7b095-110">类型</span><span class="sxs-lookup"><span data-stu-id="7b095-110">Type</span></span>|<span data-ttu-id="7b095-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b095-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b095-112">appId</span><span class="sxs-lookup"><span data-stu-id="7b095-112">appId</span></span>|<span data-ttu-id="7b095-113">String</span><span class="sxs-lookup"><span data-stu-id="7b095-113">String</span></span>|<span data-ttu-id="7b095-114">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="7b095-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b095-115">关系</span><span class="sxs-lookup"><span data-stu-id="7b095-115">Relationships</span></span>
<span data-ttu-id="7b095-116">无</span><span class="sxs-lookup"><span data-stu-id="7b095-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b095-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b095-117">JSON Representation</span></span>
<span data-ttu-id="7b095-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b095-118">Here is a JSON representation of the resource.</span></span>
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






