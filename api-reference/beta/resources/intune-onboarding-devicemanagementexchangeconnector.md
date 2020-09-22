---
title: deviceManagementExchangeConnector 资源类型
description: 表示与 Exchange 环境的连接的实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 928827e61e21629228476c3071f4f8f3e905912c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029629"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a><span data-ttu-id="8145d-103">deviceManagementExchangeConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="8145d-103">deviceManagementExchangeConnector resource type</span></span>

<span data-ttu-id="8145d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8145d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8145d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8145d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8145d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8145d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8145d-107">表示与 Exchange 环境的连接的实体。</span><span class="sxs-lookup"><span data-stu-id="8145d-107">Entity which represents a connection to an Exchange environment.</span></span>

## <a name="methods"></a><span data-ttu-id="8145d-108">方法</span><span class="sxs-lookup"><span data-stu-id="8145d-108">Methods</span></span>
|<span data-ttu-id="8145d-109">方法</span><span class="sxs-lookup"><span data-stu-id="8145d-109">Method</span></span>|<span data-ttu-id="8145d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8145d-110">Return Type</span></span>|<span data-ttu-id="8145d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8145d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8145d-112">列出 deviceManagementExchangeConnectors</span><span class="sxs-lookup"><span data-stu-id="8145d-112">List deviceManagementExchangeConnectors</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|<span data-ttu-id="8145d-113">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8145d-113">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) collection</span></span>|<span data-ttu-id="8145d-114">列出 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8145d-114">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>|
|[<span data-ttu-id="8145d-115">获取 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-115">Get deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[<span data-ttu-id="8145d-116">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-116">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="8145d-117">读取 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8145d-117">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="8145d-118">创建 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-118">Create deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[<span data-ttu-id="8145d-119">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-119">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="8145d-120">创建新的 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8145d-120">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="8145d-121">删除 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-121">Delete deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|<span data-ttu-id="8145d-122">无</span><span class="sxs-lookup"><span data-stu-id="8145d-122">None</span></span>|<span data-ttu-id="8145d-123">删除 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="8145d-123">Deletes a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>|
|[<span data-ttu-id="8145d-124">更新 deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-124">Update deviceManagementExchangeConnector</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[<span data-ttu-id="8145d-125">deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="8145d-125">deviceManagementExchangeConnector</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|<span data-ttu-id="8145d-126">更新 [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8145d-126">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>|
|[<span data-ttu-id="8145d-127">同步操作</span><span class="sxs-lookup"><span data-stu-id="8145d-127">sync action</span></span>](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|<span data-ttu-id="8145d-128">无</span><span class="sxs-lookup"><span data-stu-id="8145d-128">None</span></span>|<span data-ttu-id="8145d-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8145d-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8145d-130">属性</span><span class="sxs-lookup"><span data-stu-id="8145d-130">Properties</span></span>
|<span data-ttu-id="8145d-131">属性</span><span class="sxs-lookup"><span data-stu-id="8145d-131">Property</span></span>|<span data-ttu-id="8145d-132">类型</span><span class="sxs-lookup"><span data-stu-id="8145d-132">Type</span></span>|<span data-ttu-id="8145d-133">说明</span><span class="sxs-lookup"><span data-stu-id="8145d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8145d-134">id</span><span class="sxs-lookup"><span data-stu-id="8145d-134">id</span></span>|<span data-ttu-id="8145d-135">String</span><span class="sxs-lookup"><span data-stu-id="8145d-135">String</span></span>|<span data-ttu-id="8145d-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8145d-136">Not yet documented</span></span>|
|<span data-ttu-id="8145d-137">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8145d-137">lastSyncDateTime</span></span>|<span data-ttu-id="8145d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8145d-138">DateTimeOffset</span></span>|<span data-ttu-id="8145d-139">Exchange Connector 的上一次同步时间</span><span class="sxs-lookup"><span data-stu-id="8145d-139">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="8145d-140">status</span><span class="sxs-lookup"><span data-stu-id="8145d-140">status</span></span>|[<span data-ttu-id="8145d-141">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="8145d-141">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="8145d-142">Exchange Connector 状态。</span><span class="sxs-lookup"><span data-stu-id="8145d-142">Exchange Connector Status.</span></span> <span data-ttu-id="8145d-143">可取值为：`none`、`connectionPending`、`connected`、`disconnected`。</span><span class="sxs-lookup"><span data-stu-id="8145d-143">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="8145d-144">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="8145d-144">primarySmtpAddress</span></span>|<span data-ttu-id="8145d-145">String</span><span class="sxs-lookup"><span data-stu-id="8145d-145">String</span></span>|<span data-ttu-id="8145d-146">用于配置服务到服务 Exchange Connector 的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8145d-146">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="8145d-147">serverName</span><span class="sxs-lookup"><span data-stu-id="8145d-147">serverName</span></span>|<span data-ttu-id="8145d-148">String</span><span class="sxs-lookup"><span data-stu-id="8145d-148">String</span></span>|<span data-ttu-id="8145d-149">Exchange 服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="8145d-149">The name of the Exchange server.</span></span>|
|<span data-ttu-id="8145d-150">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="8145d-150">connectorServerName</span></span>|<span data-ttu-id="8145d-151">String</span><span class="sxs-lookup"><span data-stu-id="8145d-151">String</span></span>|<span data-ttu-id="8145d-152">托管 Exchange Connector 的服务器的名称。</span><span class="sxs-lookup"><span data-stu-id="8145d-152">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="8145d-153">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="8145d-153">exchangeConnectorType</span></span>|[<span data-ttu-id="8145d-154">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="8145d-154">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="8145d-155">配置的 Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="8145d-155">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="8145d-156">可取值为：`onPremises`、`hosted`、`serviceToService`、`dedicated`。</span><span class="sxs-lookup"><span data-stu-id="8145d-156">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="8145d-157">version</span><span class="sxs-lookup"><span data-stu-id="8145d-157">version</span></span>|<span data-ttu-id="8145d-158">String</span><span class="sxs-lookup"><span data-stu-id="8145d-158">String</span></span>|<span data-ttu-id="8145d-159">ExchangeConnectorAgent 版本</span><span class="sxs-lookup"><span data-stu-id="8145d-159">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="8145d-160">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="8145d-160">exchangeAlias</span></span>|<span data-ttu-id="8145d-161">String</span><span class="sxs-lookup"><span data-stu-id="8145d-161">String</span></span>|<span data-ttu-id="8145d-162">分配到 Exchange 服务器的别名</span><span class="sxs-lookup"><span data-stu-id="8145d-162">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="8145d-163">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="8145d-163">exchangeOrganization</span></span>|<span data-ttu-id="8145d-164">String</span><span class="sxs-lookup"><span data-stu-id="8145d-164">String</span></span>|<span data-ttu-id="8145d-165">Exchange 服务器的 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="8145d-165">Exchange Organization to the Exchange server</span></span>|

## <a name="relationships"></a><span data-ttu-id="8145d-166">关系</span><span class="sxs-lookup"><span data-stu-id="8145d-166">Relationships</span></span>
<span data-ttu-id="8145d-167">无</span><span class="sxs-lookup"><span data-stu-id="8145d-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8145d-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8145d-168">JSON Representation</span></span>
<span data-ttu-id="8145d-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8145d-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```






