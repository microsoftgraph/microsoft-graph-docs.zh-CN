---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识为网亭配置 AzureAD 组的类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16c2b17220a92f9f230b786238b1195e2af48d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849866"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="c4315-103">windowsKioskAzureADGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4315-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="c4315-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c4315-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4315-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c4315-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4315-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c4315-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4315-107">用于标识为网亭配置 AzureAD 组的类</span><span class="sxs-lookup"><span data-stu-id="c4315-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="c4315-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c4315-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4315-109">属性</span><span class="sxs-lookup"><span data-stu-id="c4315-109">Properties</span></span>
|<span data-ttu-id="c4315-110">属性</span><span class="sxs-lookup"><span data-stu-id="c4315-110">Property</span></span>|<span data-ttu-id="c4315-111">类型</span><span class="sxs-lookup"><span data-stu-id="c4315-111">Type</span></span>|<span data-ttu-id="c4315-112">说明</span><span class="sxs-lookup"><span data-stu-id="c4315-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4315-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c4315-113">displayName</span></span>|<span data-ttu-id="c4315-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c4315-114">String</span></span>|<span data-ttu-id="c4315-115">将锁定到此网亭配置 AzureAD 组的显示名称</span><span class="sxs-lookup"><span data-stu-id="c4315-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="c4315-116">groupId</span><span class="sxs-lookup"><span data-stu-id="c4315-116">groupId</span></span>|<span data-ttu-id="c4315-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c4315-117">String</span></span>|<span data-ttu-id="c4315-118">将此网亭配置到锁定的 AzureAD 组 ID</span><span class="sxs-lookup"><span data-stu-id="c4315-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4315-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="c4315-119">Relationships</span></span>
<span data-ttu-id="c4315-120">无</span><span class="sxs-lookup"><span data-stu-id="c4315-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4315-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4315-121">JSON Representation</span></span>
<span data-ttu-id="c4315-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4315-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





