---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d601e3046ba2a17426bc78ef50bd2a481d71d0cb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273527"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="e49ba-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e49ba-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="e49ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e49ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e49ba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e49ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e49ba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e49ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e49ba-107">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="e49ba-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="e49ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="e49ba-108">Properties</span></span>
|<span data-ttu-id="e49ba-109">属性</span><span class="sxs-lookup"><span data-stu-id="e49ba-109">Property</span></span>|<span data-ttu-id="e49ba-110">类型</span><span class="sxs-lookup"><span data-stu-id="e49ba-110">Type</span></span>|<span data-ttu-id="e49ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="e49ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e49ba-112">appId</span><span class="sxs-lookup"><span data-stu-id="e49ba-112">appId</span></span>|<span data-ttu-id="e49ba-113">String</span><span class="sxs-lookup"><span data-stu-id="e49ba-113">String</span></span>|<span data-ttu-id="e49ba-114">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="e49ba-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e49ba-115">关系</span><span class="sxs-lookup"><span data-stu-id="e49ba-115">Relationships</span></span>
<span data-ttu-id="e49ba-116">无</span><span class="sxs-lookup"><span data-stu-id="e49ba-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e49ba-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e49ba-117">JSON Representation</span></span>
<span data-ttu-id="e49ba-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e49ba-118">Here is a JSON representation of the resource.</span></span>
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




