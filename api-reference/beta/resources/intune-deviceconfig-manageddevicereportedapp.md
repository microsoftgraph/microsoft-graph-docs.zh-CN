---
title: managedDeviceReportedApp 资源类型
description: 用于报告功能的应用程序数据
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 104503083f5f599bc366de2ca8082fd9fdf3102e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422605"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="076f0-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="076f0-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="076f0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="076f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="076f0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="076f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="076f0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="076f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="076f0-107">用于报告功能的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="076f0-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="076f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="076f0-108">Properties</span></span>
|<span data-ttu-id="076f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="076f0-109">Property</span></span>|<span data-ttu-id="076f0-110">类型</span><span class="sxs-lookup"><span data-stu-id="076f0-110">Type</span></span>|<span data-ttu-id="076f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="076f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="076f0-112">appId</span><span class="sxs-lookup"><span data-stu-id="076f0-112">appId</span></span>|<span data-ttu-id="076f0-113">String</span><span class="sxs-lookup"><span data-stu-id="076f0-113">String</span></span>|<span data-ttu-id="076f0-114">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="076f0-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="076f0-115">关系</span><span class="sxs-lookup"><span data-stu-id="076f0-115">Relationships</span></span>
<span data-ttu-id="076f0-116">无</span><span class="sxs-lookup"><span data-stu-id="076f0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="076f0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="076f0-117">JSON Representation</span></span>
<span data-ttu-id="076f0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="076f0-118">Here is a JSON representation of the resource.</span></span>
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




