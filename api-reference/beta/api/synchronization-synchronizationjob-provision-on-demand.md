---
title: synchronizationJob： provisionOnDemand
description: 选择用户并按需预配帐户。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 26ba06868be98a6ecdc9db46d1abfc5cffefc551
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436622"
---
# <a name="synchronizationjob-provisionondemand"></a>synchronizationJob： provisionOnDemand

命名空间：microsoft.graph

选择用户并按需预配帐户。 此 API 的速率限制为每 10 秒 5 个请求。 

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     |Directory.ReadWrite.All  |
|委派（个人 Microsoft 帐户） |不支持。 |
|应用程序                            |Application.ReadWrite.OwnedBy、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|parameters|[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) 集合|表示要预配的对象和执行的同步规则。 该资源主要用于按需预配。 |



## <a name="response"></a>响应

如果成功，此方法将返回 `200 OK` 响应代码和 stringKeyStringValuePair。

## <a name="examples"></a>示例

### <a name="example-1-provision-users-from-azure-ad-to-third-party-applications"></a>示例 1：将用户从 Azure AD 预配到第三方应用程序

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand_ADto3P"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/c8c95753-f628-48e1-9fab-76c2d4cf624c/synchronization/jobs/3f7565a3-fde6-4e4d-bda8-1bb70aba3612/provisionOnDemand
Content-Type: application/json

{
  "parameters": [
    {
      "subjects": [
        {
          "objectId": "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          "objectTypeName": "User"
        }
      ],
      "ruleId": "ea807875-5618-4f0a-9125-0b46a05298ca"
    }
  ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-provisionondemand-adto3p-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-provisionondemand-adto3p-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-provisionondemand-adto3p-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-provisionondemand-adto3p-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/synchronizationjob-provisionondemand-adto3p-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/synchronizationjob-provisionondemand-adto3p-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
```
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.stringKeyStringValuePair",
    "key": "{\"result\":\"Skipped\",\"details\":{\"errorCode\":\"RedundantExport\",\"errorMessage\":\"The state of the user in both the source and target systems already match.\"}}",
    "value": "{\"action\":\"Other\",\"changeId\":\"g8ba3be8-1d7f-4a60-ae31-a8980da0a389\",\"endTime\":\"2020-06-26T13:58:24.7682084Z\",\"modifiedProperties\":[{\"displayName\":\"objectId\",\"oldValue\":null,\"newValue\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\"},{\"displayName\":\"accountEnabled\",\"oldValue\":null,\"newValue\":\"True\"},{\"displayName\":\"displayName\",\"oldValue\":null,\"newValue\":\"Bill Bob\"},{\"displayName\":\"mailNickname\",\"oldValue\":null,\"newValue\":\"Bill\"},{\"displayName\":\"userPrincipalName\",\"oldValue\":null,\"newValue\":\"BillBob@scimreftest.onmicrosoft.com\"},{\"displayName\":\"IsSoftDeleted\",\"oldValue\":null,\"newValue\":\"False\"},{\"displayName\":\"appRoleAssignments\",\"oldValue\":null,\"newValue\":\"User\"}],\"provisioningSteps\":[{\"name\":\"EntryImport\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Retrieved User 'BillBob@scimreftest.onmicrosoft.com' from Azure Active Directory\",\"timestamp\":\"2020-06-26T13:58:24.5494971Z\",\"details\":{\"objectId\":\"52cf7b7a-52be-4a9b-9c69-e4d4a4a14f76\",\"accountEnabled\":\"True\",\"displayName\":\"Fill Bob\",\"mailNickname\":\"Bill\",\"userPrincipalName\":\"BillBob@scimreftest.onmicrosoft.com\",\"IsSoftDeleted\":\"False\",\"appRoleAssignments\":\"User\"}},{\"name\":\"EntryImport\",\"type\":\"Matching\",\"status\":\"Success\",\"description\":\"Retrieved  'BillBob@scimreftest.onmicrosoft.com' from customappsso\",\"timestamp\":\"2020-06-26T13:58:24.7214072Z\",\"details\":{\"active\":\"True\",\"displayName\":\"Bill Bob\",\"externalId\":\"Bill\",\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"userName\":\"BillBob@scimreftest.onmicrosoft.com\"}},{\"name\":\"EntrySynchronizationScoping\",\"type\":\"Scoping\",\"status\":\"Success\",\"description\":\"Determine if User in scope by evaluating against each scoping filter\",\"timestamp\":\"2020-06-26T13:58:24.7526181Z\",\"details\":{\"IsActive\":\"True\",\"Assigned\":\"True\",\"IsEffectivelyEntitledForProvisioning\":\"True\",\"IsInProvisioningScopeDisplayName\":\"True\",\"ScopeEvaluationResult\":\"{}\"}},{\"name\":\"EntrySynchronizationSkip\",\"type\":\"Export\",\"status\":\"Skipped\",\"description\":\"The state of the user in both the source and target systems already match. No change to the User 'BillBob@scimreftest.onmicrosoft.com' currently needs to be made.\",\"timestamp\":\"2020-06-26T13:58:24.7682084Z\",\"details\":{\"SkipReason\":\"RedundantExport\"}}],\"reportableIdentifier\":\"BillBob@scimreftest.onmicrosoft.com\",\"startTime\":\"2020-06-26T13:58:24.5494971Z\",\"statusInfo\":{\"status\":\"Skipped\",\"errorCode\":null,\"reason\":null,\"additionalDetails\":null,\"errorCategory\":null,\"recommendedAction\":null},\"sourceIdentity\":{\"id\":\"62cf7b7a-52be-4a9b-9c69-e5d4a4a14f67\",\"type\":\"User\",\"displayName\":null,\"details\":null},\"sourceSystem\":{\"id\":null,\"name\":\"Azure Active Directory\",\"details\":null},\"targetIdentity\":{\"id\":\"52507a19-96ec-4e73-9250-3e65ffd2d926\",\"type\":\"urn:ietf:params:scim:schemas:extension:enterprise:2.0:User\",\"displayName\":null,\"details\":null},\"targetSystem\":{\"id\":null,\"name\":\"customappsso\",\"details\":null}}"
}
```

### <a name="example-2-sync-on-demand-from-active-directory-to-azure-active-directory-azure-ad-cloud-sync"></a>示例 2：按需从 Active Directory 同步到 Azure Active Directory (Azure AD 云同步) 

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand_AD2AAD"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/3e916d82-dd59-4944-824d-93092908fd8d/synchronization/jobs/264ea562-28cd-42b1-93e0-8de1f0560581/provisionOnDemand
Content-Type: application/json

{
  "parameters": [
    {
      "ruleId": "6c409270-f78a-4bc6-af23-7cf3ab6482fe",
      "subjects": [
        {
          "objectId": "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com",
          "objectTypeName": "user"
        }
      ]
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-provisionondemand-ad2aad-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-provisionondemand-ad2aad-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-provisionondemand-ad2aad-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-provisionondemand-ad2aad-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/synchronizationjob-provisionondemand-ad2aad-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/synchronizationjob-provisionondemand-ad2aad-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
```
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://syncfabric.windowsazure.com/api/$metadata#microsoft.synchronization.stringKeyStringValuePair",
    "key": "{\"result\":\"Success\",\"details\":{}}",
    "value": "{\"provisioningSteps\":[{\"name\":\"EntryImportAdd\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Received user 'adelev@chicago.com' change of type (Add) from Active Directory\",\"timestamp\":\"2022-04-21T18:40:07.8465145Z\",\"details\":{\"distinguishedName\":\"CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com\",\"cn\":\"Adele Vest\",\"originatingReplicaToken\":\"{\\\"InvocationId\\\":\\\"6cbd7b45-b262-4dad-94a3-620503ea1f25\\\",\\\"Name\\\":\\\"DC01.esf.edu\\\"}\",\"sAMAccountName\":\"adelev\",\"targetAddress\":\"SMTP:adelev@esf0.mail.onmicrosoft.com\",\"givenName\":\"Adele\",\"objectSid\":\"AQUAAAAAAAUVAAAAXAMNf/YJ8nmaUZofGG4BAA==\",\"displayName\":\"Adele Vest\",\"msExchMailboxGuid\":\"+klu7DM5yE+9tOs6MuGxsw==\",\"msExchELCMailboxFlags\":\"2\",\"pwdLastSet\":\"132772253564048004\",\"initials\":\"S\",\"msExchRecipientDisplayType\":\"-2147483642\",\"streetAddress\":\"One Microsoft Way\",\"mail\":\"adelev@chicago.com\",\"sn\":\"AdeleV\",\"msExchSafeSendersHash\":\"gny5JQ==\",\"proxyAddresses\":\"X, 5, 0,  ... X400:C=US;A= ;P=ESF;O=MAIL;S=AdeleV;G=Adele;I=S; (5)\",\"objectGUID\":\"xxxxxxxLIUuBM8qK5Sxxxx\",\"legacyExchangeDN\":\"/o=ESF/ou=External (FYDIBOHF25SPDLT)/cn=Recipients/cn=b499521b46264967a6de75f1a08add7a\",\"msExchRecipientTypeDetails\":\"2147483648\",\"userAccountControl\":\"66048\",\"accountDisabled\":\"False\",\"countryCode\":\"840\",\"co\":\"United States\",\"l\":\"Chicago\",\"extensionAttribute10\":\"839153607\",\"c\":\"US\",\"mS-DS-ConsistencyGuid\":\"xxxxxxxLIUuBM8qK5Sxxxx\",\"mailNickname\":\"adelev\",\"st\":\"NY\",\"extensionAttribute15\":\"C1EA2EA6EC56F3D94D2D89D95D70E4D0\",\"extensionAttribute14\":\"F00177677\",\"postalCode\":\"13210\",\"extensionAttribute6\":\"A5\",\"msExchRemoteRecipientType\":\"4\",\"extensionAttribute5\":\"11\",\"userPrincipalName\":\"adelev@chicago.com\",\"adminDescription\":\"\",\"company\":\"\",\"department\":\"\",\"description\":\"\",\"employeeID\":\"\",\"employeeNumber\":\"\",\"employeeType\":\"\",\"errors\":\"\",\"extensionAttribute1\":\"\",\"extensionAttribute11\":\"\",\"extensionAttribute12\":\"\",\"extensionAttribute13\":\"\",\"extensionAttribute2\":\"\",\"extensionAttribute3\":\"\",\"extensionAttribute4\":\"\",\"extensionAttribute7\":\"\",\"extensionAttribute8\":\"\",\"extensionAttribute9\":\"\",\"facsimileTelephoneNumber\":\"\",\"homePhone\":\"\",\"info\":\"\",\"ipPhone\":\"\",\"isCriticalSystemObject\":\"\",\"logs\":\"\",\"middleName\":\"\",\"mobile\":\"\",\"msDS-HABSeniorityIndex\":\"\",\"msDS-InclusionTrigger\":\"\",\"msDS-PhoneticDisplayName\":\"\",\"msDS-preferredDataLocation\":\"\",\"msExchArchiveGUID\":\"\",\"msExchArchiveName\":\"\",\"msExchAssistantName\":\"\",\"msExchAuditAdmin\":\"\",\"msExchAuditDelegate\":\"\",\"msExchAuditDelegateAdmin\":\"\",\"msExchAuditOwner\":\"\",\"msExchBlockedSendersHash\":\"\",\"msExchBypassAudit\":\"\",\"msExchELCExpirySuspensionEnd\":\"\",\"msExchELCExpirySuspensionStart\":\"\",\"msExchEnableModeration\":\"\",\"msExchExtensionCustomAttribute1\":\"\",\"msExchExtensionCustomAttribute2\":\"\",\"msExchExtensionCustomAttribute3\":\"\",\"msExchExtensionCustomAttribute4\":\"\",\"msExchExtensionCustomAttribute5\":\"\",\"msExchHideFromAddressLists\":\"\",\"msExchImmutableId\":\"\",\"msExchLitigationHoldDate\":\"\",\"msExchLitigationHoldOwner\":\"\",\"msExchMailboxAuditEnable\":\"\",\"msExchMailboxAuditLogAgeLimit\":\"\",\"msExchModerationFlags\":\"\",\"msExchRequireAuthToSendTo\":\"\",\"msExchResourceCapacity\":\"\",\"msExchResourceDisplay\":\"\",\"msExchResourceMetaData\":\"\",\"msExchResourceSearchProperties\":\"\",\"msExchRetentionComment\":\"\",\"msExchRetentionURL\":\"\",\"msExchSafeRecipientsHash\":\"\",\"msExchSenderHintTranslations\":\"\",\"msExchTeamMailboxExpiration\":\"\",\"msExchTeamMailboxSharePointUrl\":\"\",\"msExchUsageLocation\":\"\",\"msExchUserHoldPolicies\":\"\",\"msRTCSIP-ApplicationOptions\":\"\",\"mSRTCSIP-DeploymentLocator\":\"\",\"msRTCSIP-Line\":\"\",\"msRTCSIP-OptionFlags\":\"\",\"msRTCSIP-OwnerUrn\":\"\",\"msRTCSIP-PrimaryUserAddress\":\"\",\"msRTCSIP-UserEnabled\":\"\",\"objectClass\":\"\",\"otherFacsimileTelephoneNumber\":\"\",\"otherHomePhone\":\"\",\"otherIpPhone\":\"\",\"otherMobile\":\"\",\"otherPager\":\"\",\"otherTelephone\":\"\",\"pager\":\"\",\"physicalDeliveryOfficeName\":\"\",\"postOfficeBox\":\"\",\"preferredLanguage\":\"\",\"telephoneAssistant\":\"\",\"telephoneNumber\":\"\",\"thumbnailPhoto\":\"\",\"title\":\"\",\"url\":\"\",\"userCertificate\":\"\",\"userSMIMECertificate\":\"\",\"whenChanged\":\"\",\"wWWHomePage\":\"\"}},{\"name\":\"EntryImport\",\"type\":\"Import\",\"status\":\"Success\",\"description\":\"Retrieved user 'adelev@chicago.com' from Active Directory\",\"timestamp\":\"2022-04-21T18:40:07.8778004Z\",\"details\":{\"distinguishedName\":\"CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com\",\"cn\":\"Adele Vest\",\"originatingReplicaToken\":\"{\\\"InvocationId\\\":\\\"6cbd7b45-b262-4dad-94a3-620503ea1f25\\\",\\\"Name\\\":\\\"DC01.esf.edu\\\"}\",\"sAMAccountName\":\"adelev\",\"targetAddress\":\"SMTP:adelev@esf0.mail.onmicrosoft.com\",\"givenName\":\"Adele\",\"objectSid\":\"AQUAAAAAAAUVAAAAXAMNf/YJ8nmaUZofGG4BAA==\",\"displayName\":\"Adele Vest\",\"msExchMailboxGuid\":\"+klu7DM5yE+9tOs6MuGxsw==\",\"msExchELCMailboxFlags\":\"2\",\"pwdLastSet\":\"132772253564048004\",\"initials\":\"S\",\"msExchRecipientDisplayType\":\"-2147483642\",\"streetAddress\":\"One Microsoft Way\",\"mail\":\"adelev@chicago.com\",\"sn\":\"AdeleV\",\"msExchSafeSendersHash\":\"gny5JQ==\",\"proxyAddresses\":\"X, 5, 0,  ... X400:C=US;A= ;P=ESF;O=MAIL;S=AdeleV;G=Adele;I=S; (5)\",\"objectGUID\":\"xxxxxxxLIUuBM8qK5Sxxxx\",\"legacyExchangeDN\":\"/o=ESF/ou=External (FYDIBOHF25SPDLT)/cn=Recipients/cn=b499521b46264967a6de75f1a08add7a\",\"msExchRecipientTypeDetails\":\"2147483648\",\"userAccountControl\":\"66048\",\"accountDisabled\":\"False\",\"countryCode\":\"840\",\"co\":\"United States\",\"l\":\"Chicago\",\"extensionAttribute10\":\"839153607\",\"c\":\"US\",\"mS-DS-ConsistencyGuid\":\"xxxxxxxLIUuBM8qK5Sxxxx\",\"mailNickname\":\"adelev\",\"st\":\"NY\",\"extensionAttribute15\":\"C1EA2EA6EC56F3D94D2D89D95D70E4D0\",\"extensionAttribute14\":\"F00177677\",\"postalCode\":\"13210\",\"extensionAttribute6\":\"A5\",\"msExchRemoteRecipientType\":\"4\",\"extensionAttribute5\":\"11\",\"userPrincipalName\":\"adelev@chicago.com\",\"adminDescription\":\"\",\"company\":\"\",\"department\":\"\",\"description\":\"\",\"employeeID\":\"\",\"employeeNumber\":\"\",\"employeeType\":\"\",\"errors\":\"\",\"extensionAttribute1\":\"\",\"extensionAttribute11\":\"\",\"extensionAttribute12\":\"\",\"extensionAttribute13\":\"\",\"extensionAttribute2\":\"\",\"extensionAttribute3\":\"\",\"extensionAttribute4\":\"\",\"extensionAttribute7\":\"\",\"extensionAttribute8\":\"\",\"extensionAttribute9\":\"\",\"facsimileTelephoneNumber\":\"\",\"homePhone\":\"\",\"info\":\"\",\"ipPhone\":\"\",\"isCriticalSystemObject\":\"\",\"logs\":\"\",\"middleName\":\"\",\"mobile\":\"\",\"msDS-HABSeniorityIndex\":\"\",\"msDS-InclusionTrigger\":\"\",\"msDS-PhoneticDisplayName\":\"\",\"msDS-preferredDataLocation\":\"\",\"msExchArchiveGUID\":\"\",\"msExchArchiveName\":\"\",\"msExchAssistantName\":\"\",\"msExchAuditAdmin\":\"\",\"msExchAuditDelegate\":\"\",\"msExchAuditDelegateAdmin\":\"\",\"msExchAuditOwner\":\"\",\"msExchBlockedSendersHash\":\"\",\"msExchBypassAudit\":\"\",\"msExchELCExpirySuspensionEnd\":\"\",\"msExchELCExpirySuspensionStart\":\"\",\"msExchEnableModeration\":\"\",\"msExchExtensionCustomAttribute1\":\"\",\"msExchExtensionCustomAttribute2\":\"\",\"msExchExtensionCustomAttribute3\":\"\",\"msExchExtensionCustomAttribute4\":\"\",\"msExchExtensionCustomAttribute5\":\"\",\"msExchHideFromAddressLists\":\"\",\"msExchImmutableId\":\"\",\"msExchLitigationHoldDate\":\"\",\"msExchLitigationHoldOwner\":\"\",\"msExchMailboxAuditEnable\":\"\",\"msExchMailboxAuditLogAgeLimit\":\"\",\"msExchModerationFlags\":\"\",\"msExchRequireAuthToSendTo\":\"\",\"msExchResourceCapacity\":\"\",\"msExchResourceDisplay\":\"\",\"msExchResourceMetaData\":\"\",\"msExchResourceSearchProperties\":\"\",\"msExchRetentionComment\":\"\",\"msExchRetentionURL\":\"\",\"msExchSafeRecipientsHash\":\"\",\"msExchSenderHintTranslations\":\"\",\"msExchTeamMailboxExpiration\":\"\",\"msExchTeamMailboxSharePointUrl\":\"\",\"msExchUsageLocation\":\"\",\"msExchUserHoldPolicies\":\"\",\"msRTCSIP-ApplicationOptions\":\"\",\"mSRTCSIP-DeploymentLocator\":\"\",\"msRTCSIP-Line\":\"\",\"msRTCSIP-OptionFlags\":\"\",\"msRTCSIP-OwnerUrn\":\"\",\"msRTCSIP-PrimaryUserAddress\":\"\",\"msRTCSIP-UserEnabled\":\"\",\"objectClass\":\"\",\"otherFacsimileTelephoneNumber\":\"\",\"otherHomePhone\":\"\",\"otherIpPhone\":\"\",\"otherMobile\":\"\",\"otherPager\":\"\",\"otherTelephone\":\"\",\"pager\":\"\",\"physicalDeliveryOfficeName\":\"\",\"postOfficeBox\":\"\",\"preferredLanguage\":\"\",\"telephoneAssistant\":\"\",\"telephoneNumber\":\"\",\"thumbnailPhoto\":\"\",\"title\":\"\",\"url\":\"\",\"userCertificate\":\"\",\"userSMIMECertificate\":\"\",\"whenChanged\":\"\",\"wWWHomePage\":\"\"}},{\"name\":\"EntrySynchronizationScoping\",\"type\":\"Scoping\",\"status\":\"Success\",\"description\":\"Determine if user in scope by evaluating against each scoping filter\",\"timestamp\":\"2022-04-21T18:40:08.1590133Z\",\"details\":{\"Active in the source system\":\"True\",\"Scoping filter evaluation passed\":\"True\"}},{\"name\":\"EntryExportUpdate\",\"type\":\"Export\",\"status\":\"Success\",\"description\":\"User 'adelev@chicago.com' was updated in Azure Active Directory\",\"timestamp\":\"2022-04-21T18:40:09.5184649Z\",\"details\":{}}],\"modifiedProperties\":[{\"displayName\":\"AccountEnabled\",\"newValue\":\"True\"},{\"displayName\":\"Alias\",\"newValue\":\"adelev\"},{\"displayName\":\"City\",\"newValue\":\"Chicago\"},{\"displayName\":\"CommonName\",\"newValue\":\"Adele Vest\"},{\"displayName\":\"Country\",\"newValue\":\"United States\"},{\"displayName\":\"CountryCode\",\"newValue\":\"840\"},{\"displayName\":\"CountryLetterCode\",\"newValue\":\"US\"},{\"displayName\":\"DisplayName\",\"newValue\":\"Adele Vest\"},{\"displayName\":\"DnsDomainName\",\"newValue\":\"esf.edu\"},{\"displayName\":\"ExtensionAttribute10\",\"newValue\":\"839153607\"},{\"displayName\":\"ExtensionAttribute14\",\"newValue\":\"F00177677\"},{\"displayName\":\"ExtensionAttribute15\",\"newValue\":\"C1EA2EA6EC56F3D94D2D89D95D70E4D0\"},{\"displayName\":\"ExtensionAttribute5\",\"newValue\":\"11\"},{\"displayName\":\"ExtensionAttribute6\",\"newValue\":\"A5\"},{\"displayName\":\"GivenName\",\"newValue\":\"Adele\"},{\"displayName\":\"Initials\",\"newValue\":\"S\"},{\"displayName\":\"LastPasswordChangeTimestamp\",\"newValue\":\"20210927140916.0Z\"},{\"displayName\":\"LegacyExchangeDN\",\"newValue\":\"/o=ESF/ou=External (FYDIBOHF25SPDLT)/cn=Recipients/cn=b499521b46264967a6de75f1a08add7a\"},{\"displayName\":\"Mail\",\"newValue\":\"adelev@chicago.com\"},{\"displayName\":\"MSExchElcMailboxFlags\",\"newValue\":\"2\"},{\"displayName\":\"MSExchMailboxGuid\",\"newValue\":\"+klu7DM5yE+9tOs6MuGxsw==\"},{\"displayName\":\"MSExchRecipientDisplayType\",\"newValue\":\"-2147483642\"},{\"displayName\":\"MSExchRecipientTypeDetails\",\"newValue\":\"2147483648\"},{\"displayName\":\"MSExchRemoteRecipientType\",\"newValue\":\"4\"},{\"displayName\":\"MSExchSafeSendersHash\",\"newValue\":\"gny5JQ==\"},{\"displayName\":\"NetBiosName\",\"newValue\":\"ESF\"},{\"displayName\":\"OnPremisesDistinguishedName\",\"newValue\":\"CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com\"},{\"displayName\":\"OnPremiseSecurityIdentifier\",\"newValue\":\"AQUAAAAAAAUVAAAAXAMNf/YJ8nmaUZofGG4BAA==\"},{\"displayName\":\"OnPremisesSamAccountName\",\"newValue\":\"adelev\"},{\"displayName\":\"OnPremisesUserPrincipalName\",\"newValue\":\"adelev@chicago.com\"},{\"displayName\":\"PostalCode\",\"newValue\":\"13210\"},{\"displayName\":\"ProxyAddresses\",\"newValue\":\"X, 5, 0,  ... X400:C=US;A= ;P=ESF;O=MAIL;S=AdeleV;G=Adele;I=S; (5)\"},{\"displayName\":\"State\",\"newValue\":\"NY\"},{\"displayName\":\"StreetAddress\",\"newValue\":\"One Microsoft Way\"},{\"displayName\":\"Surname\",\"newValue\":\"AdeleV\"},{\"displayName\":\"TargetAddress\",\"newValue\":\"SMTP:adelev@esf0.mail.onmicrosoft.com\"},{\"displayName\":\"UserPrincipalName\",\"newValue\":\"adelev@chicago.com\"}],\"action\":\"Update\",\"changeId\":\"582595f3-53be-4843-bf0c-f57dbf8fae96\",\"endTime\":\"2022-04-21T18:40:09.5496702Z\",\"reportableIdentifier\":\"adelev@chicago.com\",\"sourceIdentity\":{\"id\":\"38a2171b-8b04-4b21-8133-ca8ae52250f3\",\"type\":\"user\"},\"sourceSystem\":{\"name\":\"Active Directory\"},\"startTime\":\"2022-04-21T18:40:07.8309453Z\",\"statusInfo\":{\"status\":\"Success\"},\"targetIdentity\":{\"id\":\"87cb2512-8e7f-4543-a9c9-e7cf8756a3ad\",\"type\":\"User\"},\"targetSystem\":{\"name\":\"Azure Active Directory\"}}"
}
```

### <a name="example-3-provision-a-group-and-two-of-its-members-on-demand"></a>示例 3：按需预配组及其两个成员

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "synchronizationjob_provisionondemand_Group"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/4e116d82-dd59-4944-824d-93091408fd8d/synchronization/jobs/664ea562-18cd-42bb-33e0-8de1f0560581/provisionOnDemand
Content-Type: application/json

{
  "parameters": [
    {
      "ruleId": "33f7c90d-bf71-41b1-bda6-aaf0ddbee5d8#V2",
      "subjects": [
        {
          "objectId": "8213fd99-d6b6-417b-8e13-af6334856215",
          "objectTypeName": "Group",
          "links": {
            "members": [
              {
                "objectId": "cbc86211-6ada-4803-b73f-8039cf56d8a2",
                "objectTypeName": "User"
              },
              {
                "objectId": "2bc86211-6ada-4803-b73f-8039cf56d8a2",
                "objectTypeName": "User"
              }
            ]
          }
        }
      ]
    }
  ]
}
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}
-->
```
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://syncfabric.windowsazure.com/api/$metadata#microsoft.synchronization.stringKeyStringValuePair",
    "key": "{\"result\":\"Success\",\"details\":{}}",
    "value": "{}"
}
```

