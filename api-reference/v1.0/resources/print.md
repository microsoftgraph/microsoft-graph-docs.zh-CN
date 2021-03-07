---
title: 打印资源类型
description: 当随附通用打印订阅时，打印功能允许管理打印机和发现可用于在通用打印中管理打印机和打印作业的 printServiceEndpoints。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: db532fed1bcdeeec749d59c8297fc36d836aed78
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517204"
---
# <a name="print-resource-type"></a><span data-ttu-id="c174f-103">打印资源类型</span><span class="sxs-lookup"><span data-stu-id="c174f-103">print resource type</span></span>

<span data-ttu-id="c174f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c174f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="c174f-105">当随附通用打印订阅时，打印功能允许管理打印机和发现可用于在通用打印中管理打印机和打印作业的[printServiceEndpoints。](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="c174f-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="c174f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c174f-106">Methods</span></span>
|<span data-ttu-id="c174f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c174f-107">Method</span></span>|<span data-ttu-id="c174f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c174f-108">Return type</span></span>|<span data-ttu-id="c174f-109">Description</span><span class="sxs-lookup"><span data-stu-id="c174f-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="c174f-110">List connectors</span><span class="sxs-lookup"><span data-stu-id="c174f-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="c174f-111">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="c174f-112">获取打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="c174f-113">列出打印机</span><span class="sxs-lookup"><span data-stu-id="c174f-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="c174f-114">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="c174f-115">获取打印机列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="c174f-116">列出共享项</span><span class="sxs-lookup"><span data-stu-id="c174f-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="c174f-117">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="c174f-118">获取打印机共享的列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="c174f-119">列出服务</span><span class="sxs-lookup"><span data-stu-id="c174f-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="c174f-120">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="c174f-121">获取服务列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-121">Get a list of services.</span></span> |
| [<span data-ttu-id="c174f-122">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="c174f-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="c174f-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="c174f-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="c174f-124">通过发布到共享集合创建新的 **打印机** 共享。</span><span class="sxs-lookup"><span data-stu-id="c174f-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="c174f-125">创建打印机</span><span class="sxs-lookup"><span data-stu-id="c174f-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="c174f-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="c174f-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="c174f-127">创建 (通用) 新打印机上注册。</span><span class="sxs-lookup"><span data-stu-id="c174f-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="c174f-128">更新设置</span><span class="sxs-lookup"><span data-stu-id="c174f-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="c174f-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="c174f-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="c174f-130">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="c174f-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="c174f-131">List taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c174f-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="c174f-132">[printTaskDefinition](printtaskdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="c174f-133">获取在通用打印中创建的 printTaskDefinitions 的租户范围列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="c174f-134">Create taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c174f-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="c174f-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c174f-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c174f-136">创建新的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="c174f-136">Create a new printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c174f-137">属性</span><span class="sxs-lookup"><span data-stu-id="c174f-137">Properties</span></span>
|<span data-ttu-id="c174f-138">属性</span><span class="sxs-lookup"><span data-stu-id="c174f-138">Property</span></span>|<span data-ttu-id="c174f-139">类型</span><span class="sxs-lookup"><span data-stu-id="c174f-139">Type</span></span>|<span data-ttu-id="c174f-140">Description</span><span class="sxs-lookup"><span data-stu-id="c174f-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c174f-141">settings</span><span class="sxs-lookup"><span data-stu-id="c174f-141">settings</span></span>|[<span data-ttu-id="c174f-142">printSettings</span><span class="sxs-lookup"><span data-stu-id="c174f-142">printSettings</span></span>](../resources/printsettings.md)|<span data-ttu-id="c174f-143">通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="c174f-143">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c174f-144">关系</span><span class="sxs-lookup"><span data-stu-id="c174f-144">Relationships</span></span>
|<span data-ttu-id="c174f-145">关系</span><span class="sxs-lookup"><span data-stu-id="c174f-145">Relationship</span></span>|<span data-ttu-id="c174f-146">类型</span><span class="sxs-lookup"><span data-stu-id="c174f-146">Type</span></span>|<span data-ttu-id="c174f-147">Description</span><span class="sxs-lookup"><span data-stu-id="c174f-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c174f-148">服务</span><span class="sxs-lookup"><span data-stu-id="c174f-148">services</span></span>|<span data-ttu-id="c174f-149">[printService](printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-149">[printService](printservice.md) collection</span></span>|<span data-ttu-id="c174f-150">可用通用打印服务终结点的列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-150">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="c174f-151">打印机</span><span class="sxs-lookup"><span data-stu-id="c174f-151">printers</span></span>|<span data-ttu-id="c174f-152">[打印机](printer.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-152">[printer](printer.md) collection</span></span>|<span data-ttu-id="c174f-153">在租户中注册的打印机列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-153">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="c174f-154">shares</span><span class="sxs-lookup"><span data-stu-id="c174f-154">shares</span></span>|<span data-ttu-id="c174f-155">[printerShare](printershare.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-155">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="c174f-156">在租户中注册的打印机共享列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-156">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="c174f-157">连接器</span><span class="sxs-lookup"><span data-stu-id="c174f-157">connectors</span></span>|<span data-ttu-id="c174f-158">[printConnector](printconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-158">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="c174f-159">可用打印连接器的列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-159">The list of available print connectors.</span></span>|
|<span data-ttu-id="c174f-160">operations</span><span class="sxs-lookup"><span data-stu-id="c174f-160">operations</span></span>|<span data-ttu-id="c174f-161">[printOperation](../resources/printoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-161">[printOperation](../resources/printoperation.md) collection</span></span>|<span data-ttu-id="c174f-162">长时间运行的打印操作的列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-162">The list of print long running operations.</span></span>|
|<span data-ttu-id="c174f-163">服务</span><span class="sxs-lookup"><span data-stu-id="c174f-163">services</span></span>|<span data-ttu-id="c174f-164">[printService](../resources/printservice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-164">[printService](../resources/printservice.md) collection</span></span>|<span data-ttu-id="c174f-165">打印基础结构的各个组件的打印服务实例列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-165">The list of print service instances for various components of the printing infrastructure.</span></span>|
|<span data-ttu-id="c174f-166">taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c174f-166">taskDefinitions</span></span>|<span data-ttu-id="c174f-167">[printTaskDefinition](../resources/printtaskdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c174f-167">[printTaskDefinition](../resources/printtaskdefinition.md) collection</span></span>|<span data-ttu-id="c174f-168">在通用打印中发生各种事件时可以触发的任务的抽象定义列表。</span><span class="sxs-lookup"><span data-stu-id="c174f-168">List of abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c174f-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c174f-169">JSON representation</span></span>
<span data-ttu-id="c174f-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c174f-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

