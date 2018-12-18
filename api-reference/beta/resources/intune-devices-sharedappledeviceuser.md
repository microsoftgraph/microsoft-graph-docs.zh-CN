---
title: sharedAppleDeviceUser 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 4e16d691ed6286fb8046c0693292012e1e94a0ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315986"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="e9f85-103">sharedAppleDeviceUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9f85-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="e9f85-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e9f85-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9f85-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9f85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9f85-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9f85-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9f85-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e9f85-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e9f85-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9f85-108">Properties</span></span>
|<span data-ttu-id="e9f85-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9f85-109">Property</span></span>|<span data-ttu-id="e9f85-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9f85-110">Type</span></span>|<span data-ttu-id="e9f85-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9f85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f85-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9f85-112">userPrincipalName</span></span>|<span data-ttu-id="e9f85-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e9f85-113">String</span></span>|<span data-ttu-id="e9f85-114">用户名</span><span class="sxs-lookup"><span data-stu-id="e9f85-114">User name</span></span>|
|<span data-ttu-id="e9f85-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="e9f85-115">dataToSync</span></span>|<span data-ttu-id="e9f85-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9f85-116">Boolean</span></span>|<span data-ttu-id="e9f85-117">数据同步</span><span class="sxs-lookup"><span data-stu-id="e9f85-117">Data to sync</span></span>|
|<span data-ttu-id="e9f85-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="e9f85-118">dataQuota</span></span>|<span data-ttu-id="e9f85-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e9f85-119">Int64</span></span>|<span data-ttu-id="e9f85-120">数据配额</span><span class="sxs-lookup"><span data-stu-id="e9f85-120">Data quota</span></span>|
|<span data-ttu-id="e9f85-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="e9f85-121">dataUsed</span></span>|<span data-ttu-id="e9f85-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e9f85-122">Int64</span></span>|<span data-ttu-id="e9f85-123">数据配额</span><span class="sxs-lookup"><span data-stu-id="e9f85-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9f85-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="e9f85-124">Relationships</span></span>
<span data-ttu-id="e9f85-125">无</span><span class="sxs-lookup"><span data-stu-id="e9f85-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9f85-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9f85-126">JSON Representation</span></span>
<span data-ttu-id="e9f85-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9f85-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





