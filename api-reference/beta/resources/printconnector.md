---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 PrintConnector 资源可用于查看连接器状态和更新属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 9962bad290d6a07c214107e58c8a96afb9148394
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727988"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="fa0ca-104">printConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa0ca-104">printConnector resource type</span></span>

<span data-ttu-id="fa0ca-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa0ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa0ca-106">表示已使用通用打印订阅注册的打印连接器。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="fa0ca-107">PrintConnector 资源可用于查看连接器状态和更新属性。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="fa0ca-108">Methods</span><span class="sxs-lookup"><span data-stu-id="fa0ca-108">Methods</span></span>

| <span data-ttu-id="fa0ca-109">方法</span><span class="sxs-lookup"><span data-stu-id="fa0ca-109">Method</span></span>       | <span data-ttu-id="fa0ca-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fa0ca-110">Return Type</span></span> | <span data-ttu-id="fa0ca-111">说明</span><span class="sxs-lookup"><span data-stu-id="fa0ca-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fa0ca-112">Get connector</span><span class="sxs-lookup"><span data-stu-id="fa0ca-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="fa0ca-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="fa0ca-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="fa0ca-114">读取连接器对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="fa0ca-115">更新连接器</span><span class="sxs-lookup"><span data-stu-id="fa0ca-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="fa0ca-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="fa0ca-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="fa0ca-117">更新连接器对象。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-117">Update the connector object.</span></span> |
| [<span data-ttu-id="fa0ca-118">删除连接器</span><span class="sxs-lookup"><span data-stu-id="fa0ca-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="fa0ca-119">无</span><span class="sxs-lookup"><span data-stu-id="fa0ca-119">None</span></span> | <span data-ttu-id="fa0ca-120">从通用打印服务中注销连接器。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="fa0ca-121">属性</span><span class="sxs-lookup"><span data-stu-id="fa0ca-121">Properties</span></span>
| <span data-ttu-id="fa0ca-122">属性</span><span class="sxs-lookup"><span data-stu-id="fa0ca-122">Property</span></span>     | <span data-ttu-id="fa0ca-123">类型</span><span class="sxs-lookup"><span data-stu-id="fa0ca-123">Type</span></span>        | <span data-ttu-id="fa0ca-124">说明</span><span class="sxs-lookup"><span data-stu-id="fa0ca-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fa0ca-125">id</span><span class="sxs-lookup"><span data-stu-id="fa0ca-125">id</span></span>|<span data-ttu-id="fa0ca-126">String</span><span class="sxs-lookup"><span data-stu-id="fa0ca-126">String</span></span>| <span data-ttu-id="fa0ca-127">只读。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-127">Read-only.</span></span>|
|<span data-ttu-id="fa0ca-128">displayName</span><span class="sxs-lookup"><span data-stu-id="fa0ca-128">displayName</span></span>|<span data-ttu-id="fa0ca-129">String</span><span class="sxs-lookup"><span data-stu-id="fa0ca-129">String</span></span>|<span data-ttu-id="fa0ca-130">连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-130">The name of the connector.</span></span>|
|<span data-ttu-id="fa0ca-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="fa0ca-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="fa0ca-132">String</span><span class="sxs-lookup"><span data-stu-id="fa0ca-132">String</span></span>|<span data-ttu-id="fa0ca-133">连接器计算机的主机名。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="fa0ca-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="fa0ca-134">operatingSystem</span></span>|<span data-ttu-id="fa0ca-135">String</span><span class="sxs-lookup"><span data-stu-id="fa0ca-135">String</span></span>|<span data-ttu-id="fa0ca-136">连接器计算机的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="fa0ca-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="fa0ca-137">appVersion</span></span>|<span data-ttu-id="fa0ca-138">String</span><span class="sxs-lookup"><span data-stu-id="fa0ca-138">String</span></span>|<span data-ttu-id="fa0ca-139">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-139">The connector's version.</span></span>|
|<span data-ttu-id="fa0ca-140">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="fa0ca-140">deviceHealth</span></span>|[<span data-ttu-id="fa0ca-141">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="fa0ca-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="fa0ca-142">连接器的设备运行状况。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-142">The connector's device health.</span></span>|
|<span data-ttu-id="fa0ca-143">location</span><span class="sxs-lookup"><span data-stu-id="fa0ca-143">location</span></span>|[<span data-ttu-id="fa0ca-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="fa0ca-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="fa0ca-145">连接器的物理位置和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="fa0ca-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="fa0ca-146">registeredDateTime</span></span>|<span data-ttu-id="fa0ca-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa0ca-147">DateTimeOffset</span></span>|<span data-ttu-id="fa0ca-148">注册连接器时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="fa0ca-149">registeredBy</span><span class="sxs-lookup"><span data-stu-id="fa0ca-149">registeredBy</span></span>|[<span data-ttu-id="fa0ca-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="fa0ca-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="fa0ca-151">注册了连接器的用户。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa0ca-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa0ca-152">JSON representation</span></span>

<span data-ttu-id="fa0ca-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa0ca-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


