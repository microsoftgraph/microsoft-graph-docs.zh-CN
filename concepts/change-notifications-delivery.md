---
title: 以不同方式接收更改通知
description: 更改通知可以通过不同的技术来传送，包括 Webhook 和 Azure 事件中心。
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20, devx-track-azurecli
ms.openlocfilehash: 59caceb3b56853b9bc4d20fa97cfc035b1a3ea0c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134064"
---
# <a name="get-change-notifications-delivered-in-different-ways"></a>以不同方式接收更改通知

可通过不同方式向订阅者传送更改通知。如果更改通知的主要传送模式是 Webhook，则对于高吞吐量场景或当接收方无法公开公用的通知 URL 时，利用 Webhooks 可能很困难。  

此更改通知传递模式可用于支持 Microsoft Graph 更改通知的所有资源。

高吞吐量场景的恰当例子包括订阅大量资源的应用程序、订阅频繁变更的资源的应用程序以及跨大量组织订阅资源的多租户应用程序。

## <a name="using-azure-event-hubs-to-receive-change-notifications"></a>使用 Azure 事件中心接收更改通知

[Azure 事件中心](https://azure.microsoft.com/services/event-hubs)是专为大规模部署而构建的常用实时事件引入和分发服务。 你可以使用 Azure 事件中心而不是传统 Webhook 来接收更改通知。  
使用 Azure 事件中心接收更改通知与 Webhook 在某些方面有所不同，包括：

- 不依赖公开显示的通知 URL。 事件中心 SDK 会将通知转发到你的应用程序。
- 无需恢复[通知 URL 验证](webhooks.md#notification-endpoint-validation)。 可忽略收到的验证消息。
- 需要预配 Azure 事件中心。
- 需要预配 Azure 密钥保管库。

### <a name="set-up-the-azure-keyvault-and-azure-event-hubs"></a>设置 Azure 密钥保管库和 Azure 事件中心

本节将指导你完成所需的 Azure 服务设置。

#### <a name="option-1-using-the-azure-cli"></a>选项 1：使用 Azure CLI

[Azure CLI](/cli/azure/what-is-azure-cli) 允许你在 Azure 中编写脚本并自动执行管理任务。 可以[在本地计算机上安装](/cli/azure/install-azure-cli) CLI 或直接从 [Azure Cloud Shell](/azure/cloud-shell/quickstart) 运行。

```azurecli
# --------------
# TODO: update the following values
#sets the name of the resource group
resourcegroup=rg-graphevents-dev
#sets the location of the resources
location='uk south'
#sets the name of the Azure Event Hubs namespace
evhamespacename=evh-graphevents-dev
#sets the name of the hub under the namespace
evhhubname=graphevents
#sets the name of the access policy to the hub
evhpolicyname=grapheventspolicy
#sets the name of the Azure KeyVault
keyvaultname=kv-graphevents
#sets the name of the secret in Azure KeyVault that will contain the connection string to the hub
keyvaultsecretname=grapheventsconnectionstring
# --------------
az group create --location $location --name $resourcegroup
az eventhubs namespace create --name $evhamespacename --resource-group $resourcegroup --sku Basic --location $location
az eventhubs eventhub create --name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --partition-count 2 --message-retention 1
az eventhubs eventhub authorization-rule create --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --rights Send
evhprimaryconnectionstring=`az eventhubs eventhub authorization-rule keys list --name $evhpolicyname --eventhub-name $evhhubname --namespace-name $evhamespacename --resource-group $resourcegroup --query "primaryConnectionString" --output tsv`
az keyvault create --name $keyvaultname --resource-group $resourcegroup --location $location --enable-soft-delete true --sku standard --retention-days 90
az keyvault secret set --name $keyvaultsecretname --value $evhprimaryconnectionstring --vault-name $keyvaultname --output none
graphspn=`az ad sp list --display-name 'Microsoft Graph Change Tracking' --query "[].appId" --output tsv`
az keyvault set-policy --name $keyvaultname --resource-group $resourcegroup --secret-permissions get --spn $graphspn --output none
keyvaulturi=`az keyvault show --name $keyvaultname --resource-group $resourcegroup --query "properties.vaultUri" --output tsv`
domainname=`az ad signed-in-user show --query 'userPrincipalName' | cut -d '@' -f 2 | sed 's/\"//'`
notificationUrl="EventHub:${keyvaulturi}secrets/${keyvaultsecretname}?tenantId=${domainname}"
echo "Notification Url:\n${notificationUrl}"
```

> **注意：** 此处提供的脚本与基于 Linux 的 命令行管理程序、Windows WSL 和 Azure Cloud Shell 兼容。 它要求在 Windows 命令行管理程序中运行某些更新。

#### <a name="option-2-using-the-azure-portal"></a>选项 2：使用 Azure 门户

##### <a name="configuring-the-azure-event-hub"></a>配置 Azure 事件中心

在本节中，你将：

- 创建 Azure 事件中心命名空间。
- 将中心添加到将转发和传送通知的该命名空间。
- 添加共享访问策略，它将允许你获取新创建的中心的连接字符串。

步骤：

1. 打开浏览器以访问 [Azure 门户](https://portal.azure.com)。
1. 选择“**创建资源**”。
1. 在搜索栏中键入“**事件中心**”。
1. 选择“**事件中心**”建议。 此时将加载“创建事件中心”页面。  
1. 在“创建事件中心”页面上，单击“**创建**”。
1. 填写事件中心命名空间创建详细信息，然后单击“**创建**”。  
1. 预配事件中心命名空间后，转到该命名空间的页面。  
1. 单击“**事件中心**”和“**+ 事件中心**”。  
1. 为新事件中心命名，然后单击“**创建**”。  
1. 创建事件中心后，单击事件中心的名称，然后单击“**共享访问策略**”和“**+ 添加**”以添加新策略。  
1. 为策略命名，选中“**发送**”，然后单击“**创建**”。  
1. 创建策略后，单击策略的名称以打开“详细信息”面板，然后复制“**连接字符串-主键**” 值。 记下该值，在下一步中你需要使用它。  

##### <a name="configuring-the-azure-key-vault"></a>配置 Azure 密钥保管库

为了安全地访问事件中心并允许密钥轮换，Microsoft Graph 将通过 Azure 密钥保管库获取事件中心的连接字符串。  
在本节中，你将：

- 创建 Azure 密钥保管库以存储密钥。
- 将连接字符串作为密钥添加到事件中心。
- 为 Microsoft Graph 添加访问策略以访问密钥。

步骤：

1. 打开浏览器以访问 [Azure 门户](https://portal.azure.com)。
1. 选择“**创建资源**”。
1. 在搜索栏中键入“**密钥保管库**”。
1. 选择“**密钥保管库**”建议。 此时将加载“创建密钥保管库”页面。
1. 在“创建密钥保管库”页面上，单击“**创建**”。  
1. 填写密钥保管库创建详细信息，然后单击“**审阅 + 创建**”和“**创建**”。  
1. 使用通知中的“**转到资源**”转到新创建的密钥保管库。  
1. 复制 **DNS 名称**；在下一步中你需要使用它。  
1. 转到“**密钥**”，然后单击“**+ 生成/导入**”。  
1. 为密钥命名，并保留名称供以后使用，在下一步中你需要使用它。 对于该值，请粘贴在“事件中心”步骤中生成的连接字符串。 单击“**创建**”。  
1. 单击“**访问策略**”和“**+ 添加访问策略**”。  
1. 对于“**密钥权限**”，选择“**获取**”；对于“**选择主体**”，选择“**Microsoft Graph 更改跟踪**”。 单击“**添加**”。  

### <a name="creating-the-subscription-and-receiving-notifications"></a>创建订阅并接收通知

创建所需的 Azure 密钥保管库和 Azure 事件中心服务后，你将能够创建订阅并开始通过 Azure 事件中心接收更改通知。

#### <a name="creating-the-subcription"></a>创建订阅

使用事件中心订阅更改通知与使用 Webhook 订阅更改通知几乎相同。 主要区别在于前者依赖事件中心来传送通知。 所有其他操作都类似，包括[创建订阅](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)。  

创建订阅期间的主要区别是 **notificationUrl**。 必须将其设置为 `EventHub:https://<azurekeyvaultname>.vault.azure.net/secrets/<secretname>?tenantId=<domainname>`，并使用以下值：

- `azurekeyvaultname` - 创建密钥保管库时为其提供的名称。 可在 DNS 名称中找到它。
- `secretname` - 创建密钥时为其提供的名称。 可在 Azure 密钥保管库的“**密钥**”页面上找到它。
- `domainname` - 租户的名称；例如，consto.onmicrosoft.com 或 contoso.com。 由于此域将用于访问 Azure 密钥保管库，因此请务必使其与包含 Azure 密钥保管库的 Azure 订阅所使用的域相匹配。 若要获取此信息，可转到你创建的 Azure 密钥保管库的概述页面，并单击该订阅。 域名将显示在“**目录**”字段下。

#### <a name="receiving-notifications"></a>接收通知

事件现在将通过事件中心传送到你的应用程序中。 有关详细信息，请参阅事件中心文档中的[接收事件](/azure/event-hubs/get-started-dotnet-standard-send-v2#receive-events)。

在应用程序中接收通知之前，你需要创建另一个具有“侦听”权限的共享访问策略并获取连接字符串，类似于[配置 Azure 事件中心](#configuring-the-azure-event-hub)中列出的步骤。

> **注意：** 为应用程序创建单独的策略来侦听事件中心消息，而不是重用在 Azure 密钥保管库中设置的相同连接字符串。 这可确保解决方案的每个组件仅具有所需的权限，并遵循最低权限安全原则。

> **注意：** 应用程序会在每次创建新订阅时收到验证消息。 应忽略这些通知。 下面的示例表示验证消息的正文。

```json
 {
    "value":[
        {
            "subscriptionId":"NA",
            "subscriptionExpirationDateTime":"NA",
            "clientState":"NA",
            "changeType":"Validation: Testing client application reachability for subscription Request-Id: 522a8e7e-096a-494c-aaf1-ac0dcfca45b7",
            "resource":"NA",
            "resourceData":{
                "@odata.type":"NA",
                "@odata.id":"NA",
                "id":"NA"
            }
        }
    ]
}
```

### <a name="what-happens-if-the-microsoft-graph-change-tracking-application-is-missing"></a>如果缺少 Microsoft Graph 更改跟踪应用程序会怎样？

租户中可能缺少 **Microsoft Graph 更改跟踪** 服务主体，这取决于租户的创建时间和管理操作。 要解决此问题，请在 [Microsoft Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer) 中运行 [以下查询](https://developer.microsoft.com/en-us/graph/graph-explorer?request=servicePrincipals&method=POST&version=v1.0&GraphUrl=https://graph.microsoft.com&requestBody=eyJhcHBJZCI6IjBiZjMwZjNiLTRhNTItNDhkZi05YTgyLTIzNDkxMGM0YTA4NiJ9)。

查询详细信息：

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals
{
    "appId": "0bf30f3b-4a52-48df-9a82-234910c4a086"
}
```

> **注意：** 运行此查询会导致访问被拒绝。 在这种情况下，请选择左上角帐户名称旁边的齿轮图标。 然后选择“**选择权限**”并搜索 **Application.ReadWrite.All**。 检查权限，然后选择“**同意**”。 同意此新权限后，再次运行请求。

> **注意：** 此 API 仅适用于学校或工作帐户，而不适用于个人帐户。 请确保使用域中的帐户登录。

或者，你也可以使用此 [Azure Active Directory PowerShell](/powershell/azure/active-directory/install-adv2?view=azureadps-2.0) 脚本添加缺少的服务主体。

```PowerShell
Connect-AzureAD -TenantId <tenant-id>
# replace tenant-id by the id of your tenant.
New-AzureADServicePrincipal -AppId 0bf30f3b-4a52-48df-9a82-234910c4a086
```

## <a name="next-steps"></a>后续步骤

请参阅下面的 Azure 事件中心快速入门：

- [.NET Core](/azure/event-hubs/get-started-dotnet-standard-send-v2)
- [Java](/azure/event-hubs/event-hubs-java-get-started-send)
- [Python](/azure/event-hubs/get-started-python-send-v2)
- [JavaScript](/azure/event-hubs/get-started-node-send-v2)
