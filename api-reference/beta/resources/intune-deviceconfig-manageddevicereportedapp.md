---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6704e4f2f8796be6c246d6deb6f5e0e8821ba411
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788609"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="8e3ab-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e3ab-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="8e3ab-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e3ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e3ab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e3ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e3ab-106">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="8e3ab-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="8e3ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="8e3ab-107">Properties</span></span>
|<span data-ttu-id="8e3ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e3ab-108">Property</span></span>|<span data-ttu-id="8e3ab-109">类型</span><span class="sxs-lookup"><span data-stu-id="8e3ab-109">Type</span></span>|<span data-ttu-id="8e3ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="8e3ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3ab-111">appId</span><span class="sxs-lookup"><span data-stu-id="8e3ab-111">appId</span></span>|<span data-ttu-id="8e3ab-112">String</span><span class="sxs-lookup"><span data-stu-id="8e3ab-112">String</span></span>|<span data-ttu-id="8e3ab-113">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="8e3ab-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e3ab-114">关系</span><span class="sxs-lookup"><span data-stu-id="8e3ab-114">Relationships</span></span>
<span data-ttu-id="8e3ab-115">无</span><span class="sxs-lookup"><span data-stu-id="8e3ab-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e3ab-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e3ab-116">JSON Representation</span></span>
<span data-ttu-id="8e3ab-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e3ab-117">Here is a JSON representation of the resource.</span></span>
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



