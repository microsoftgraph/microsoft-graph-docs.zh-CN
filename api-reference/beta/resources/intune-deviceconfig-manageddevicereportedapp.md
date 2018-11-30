---
title: managedDeviceReportedApp 资源类型
description: 用于报告功能的应用程序数据
ms.openlocfilehash: 820269422891e01352a7f605d62147a84facea67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042307"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="448b7-103">managedDeviceReportedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="448b7-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="448b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="448b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="448b7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="448b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="448b7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="448b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="448b7-107">用于报告功能的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="448b7-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="448b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="448b7-108">Properties</span></span>
|<span data-ttu-id="448b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="448b7-109">Property</span></span>|<span data-ttu-id="448b7-110">类型</span><span class="sxs-lookup"><span data-stu-id="448b7-110">Type</span></span>|<span data-ttu-id="448b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="448b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="448b7-112">appId</span><span class="sxs-lookup"><span data-stu-id="448b7-112">appId</span></span>|<span data-ttu-id="448b7-113">String</span><span class="sxs-lookup"><span data-stu-id="448b7-113">String</span></span>|<span data-ttu-id="448b7-114">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="448b7-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="448b7-115">关系</span><span class="sxs-lookup"><span data-stu-id="448b7-115">Relationships</span></span>
<span data-ttu-id="448b7-116">无</span><span class="sxs-lookup"><span data-stu-id="448b7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="448b7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="448b7-117">JSON Representation</span></span>
<span data-ttu-id="448b7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="448b7-118">Here is a JSON representation of the resource.</span></span>
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





