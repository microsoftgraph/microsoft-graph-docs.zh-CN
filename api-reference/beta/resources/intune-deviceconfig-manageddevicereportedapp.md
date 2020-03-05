---
title: managedDeviceReportedApp 资源类型
description: 用于报告的应用程序数据
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff42634a69ce9c7ea3c2e54e88401b8041348fc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526046"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="56415-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="56415-103">managedDeviceReportedApp resource type</span></span>

<span data-ttu-id="56415-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="56415-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56415-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56415-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56415-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56415-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56415-107">用于报告的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="56415-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="56415-108">属性</span><span class="sxs-lookup"><span data-stu-id="56415-108">Properties</span></span>
|<span data-ttu-id="56415-109">属性</span><span class="sxs-lookup"><span data-stu-id="56415-109">Property</span></span>|<span data-ttu-id="56415-110">类型</span><span class="sxs-lookup"><span data-stu-id="56415-110">Type</span></span>|<span data-ttu-id="56415-111">说明</span><span class="sxs-lookup"><span data-stu-id="56415-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56415-112">appId</span><span class="sxs-lookup"><span data-stu-id="56415-112">appId</span></span>|<span data-ttu-id="56415-113">String</span><span class="sxs-lookup"><span data-stu-id="56415-113">String</span></span>|<span data-ttu-id="56415-114">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="56415-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="56415-115">关系</span><span class="sxs-lookup"><span data-stu-id="56415-115">Relationships</span></span>
<span data-ttu-id="56415-116">无</span><span class="sxs-lookup"><span data-stu-id="56415-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56415-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56415-117">JSON Representation</span></span>
<span data-ttu-id="56415-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56415-118">Here is a JSON representation of the resource.</span></span>
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



