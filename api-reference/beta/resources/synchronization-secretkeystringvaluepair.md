---
title: synchronizationSecretKeyStringValuePair 资源类型
description: 表示单个密码值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: da408988c61ffa8d608fe7f36b5925107731d714
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129366"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="7cff2-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="7cff2-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="7cff2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cff2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cff2-105">表示单个密码值。</span><span class="sxs-lookup"><span data-stu-id="7cff2-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="7cff2-106">属性</span><span class="sxs-lookup"><span data-stu-id="7cff2-106">Properties</span></span>
| <span data-ttu-id="7cff2-107">属性</span><span class="sxs-lookup"><span data-stu-id="7cff2-107">Property</span></span>     | <span data-ttu-id="7cff2-108">类型</span><span class="sxs-lookup"><span data-stu-id="7cff2-108">Type</span></span>   |<span data-ttu-id="7cff2-109">说明</span><span class="sxs-lookup"><span data-stu-id="7cff2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cff2-110">Key</span><span class="sxs-lookup"><span data-stu-id="7cff2-110">key</span></span>|<span data-ttu-id="7cff2-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7cff2-111">String</span></span>| <span data-ttu-id="7cff2-112">可能的值是： `None` ， ， ， ， ， `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer` `ValidateDomain` `TestReferences` 。</span><span class="sxs-lookup"><span data-stu-id="7cff2-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="7cff2-113">value</span><span class="sxs-lookup"><span data-stu-id="7cff2-113">value</span></span>|<span data-ttu-id="7cff2-114">String</span><span class="sxs-lookup"><span data-stu-id="7cff2-114">String</span></span>|<span data-ttu-id="7cff2-115">密码的值。</span><span class="sxs-lookup"><span data-stu-id="7cff2-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cff2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cff2-116">JSON representation</span></span>

<span data-ttu-id="7cff2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cff2-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


