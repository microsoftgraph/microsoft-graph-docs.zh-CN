---
title: macOSFirewallApplication 资源类型
description: 表示 macOS 防火墙应用程序列表中的应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45d8742a888eb492b71bf9829b9621bde9608ef5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794965"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="64044-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="64044-103">macOSFirewallApplication resource type</span></span>

> <span data-ttu-id="64044-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64044-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64044-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64044-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64044-106">表示 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="64044-106">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="64044-107">属性</span><span class="sxs-lookup"><span data-stu-id="64044-107">Properties</span></span>
|<span data-ttu-id="64044-108">属性</span><span class="sxs-lookup"><span data-stu-id="64044-108">Property</span></span>|<span data-ttu-id="64044-109">类型</span><span class="sxs-lookup"><span data-stu-id="64044-109">Type</span></span>|<span data-ttu-id="64044-110">说明</span><span class="sxs-lookup"><span data-stu-id="64044-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64044-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="64044-111">bundleId</span></span>|<span data-ttu-id="64044-112">String</span><span class="sxs-lookup"><span data-stu-id="64044-112">String</span></span>|<span data-ttu-id="64044-113">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="64044-113">BundleId of the application.</span></span>|
|<span data-ttu-id="64044-114">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="64044-114">allowsIncomingConnections</span></span>|<span data-ttu-id="64044-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="64044-115">Boolean</span></span>|<span data-ttu-id="64044-116">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="64044-116">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64044-117">关系</span><span class="sxs-lookup"><span data-stu-id="64044-117">Relationships</span></span>
<span data-ttu-id="64044-118">无</span><span class="sxs-lookup"><span data-stu-id="64044-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64044-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64044-119">JSON Representation</span></span>
<span data-ttu-id="64044-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64044-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





