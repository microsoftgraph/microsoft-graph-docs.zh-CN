---
title: macOSFirewallApplication 资源类型
description: 表示 macOS 防火墙应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ad576bb4cd6f23919d927797708786413c703de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024162"
---
# <a name="macosfirewallapplication-resource-type"></a><span data-ttu-id="2554e-103">macOSFirewallApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="2554e-103">macOSFirewallApplication resource type</span></span>

<span data-ttu-id="2554e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2554e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2554e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2554e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2554e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2554e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2554e-107">表示 macOS 防火墙应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="2554e-107">Represents an app in the list of macOS firewall applications</span></span>

## <a name="properties"></a><span data-ttu-id="2554e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2554e-108">Properties</span></span>
|<span data-ttu-id="2554e-109">属性</span><span class="sxs-lookup"><span data-stu-id="2554e-109">Property</span></span>|<span data-ttu-id="2554e-110">类型</span><span class="sxs-lookup"><span data-stu-id="2554e-110">Type</span></span>|<span data-ttu-id="2554e-111">说明</span><span class="sxs-lookup"><span data-stu-id="2554e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2554e-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="2554e-112">bundleId</span></span>|<span data-ttu-id="2554e-113">String</span><span class="sxs-lookup"><span data-stu-id="2554e-113">String</span></span>|<span data-ttu-id="2554e-114">应用程序的 BundleId。</span><span class="sxs-lookup"><span data-stu-id="2554e-114">BundleId of the application.</span></span>|
|<span data-ttu-id="2554e-115">allowsIncomingConnections</span><span class="sxs-lookup"><span data-stu-id="2554e-115">allowsIncomingConnections</span></span>|<span data-ttu-id="2554e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2554e-116">Boolean</span></span>|<span data-ttu-id="2554e-117">是否允许传入连接。</span><span class="sxs-lookup"><span data-stu-id="2554e-117">Whether or not incoming connections are allowed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2554e-118">关系</span><span class="sxs-lookup"><span data-stu-id="2554e-118">Relationships</span></span>
<span data-ttu-id="2554e-119">无</span><span class="sxs-lookup"><span data-stu-id="2554e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2554e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2554e-120">JSON Representation</span></span>
<span data-ttu-id="2554e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2554e-121">Here is a JSON representation of the resource.</span></span>
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






