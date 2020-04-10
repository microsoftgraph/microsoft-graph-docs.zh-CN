---
title: synchronizationSecretKeyStringValuePair 资源类型
description: 表示单个机密值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b2c5929b7ba00a12cf66cd3f013dbf31446aba19
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217582"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="9d954-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d954-103">synchronizationSecretKeyStringValuePair resource type</span></span>

<span data-ttu-id="9d954-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d954-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d954-105">表示单个机密值。</span><span class="sxs-lookup"><span data-stu-id="9d954-105">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="9d954-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d954-106">Properties</span></span>
| <span data-ttu-id="9d954-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d954-107">Property</span></span>     | <span data-ttu-id="9d954-108">类型</span><span class="sxs-lookup"><span data-stu-id="9d954-108">Type</span></span>   |<span data-ttu-id="9d954-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d954-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d954-110">Key</span><span class="sxs-lookup"><span data-stu-id="9d954-110">key</span></span>|<span data-ttu-id="9d954-111">字符串</span><span class="sxs-lookup"><span data-stu-id="9d954-111">String</span></span>| <span data-ttu-id="9d954-112">可能的值为`None`： `UserName`、 `Password`、 `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ValidateDomain` `TestReferences`、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、、。 `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken` `SyncAll` `InstanceName` `Oauth2ClientId` `Oauth2ClientSecret` `CompanyId` `UpdateKeyOnSoftDelete` `SynchronizationSchedule` `SystemOfRecord` `SandboxName` `EnforceDomain` `SyncNotificationSettings` `Server` `PerformInboundEntitlementGrants` `HardDeletesEnabled` `SyncAgentCompatibilityKey` `SyncAgentADContainer`</span><span class="sxs-lookup"><span data-stu-id="9d954-112">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="9d954-113">value</span><span class="sxs-lookup"><span data-stu-id="9d954-113">value</span></span>|<span data-ttu-id="9d954-114">String</span><span class="sxs-lookup"><span data-stu-id="9d954-114">String</span></span>|<span data-ttu-id="9d954-115">密码的值。</span><span class="sxs-lookup"><span data-stu-id="9d954-115">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d954-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d954-116">JSON representation</span></span>

<span data-ttu-id="9d954-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d954-117">The following is a JSON representation of the resource.</span></span>

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
