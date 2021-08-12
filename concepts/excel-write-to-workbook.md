---
title: 使用 Microsoft Graph 将数据写入 Excel 工作簿
description: q=excelstarter)。
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 60f9b32cc6f769b309d64d5661781840b878e36605e63757f04b9538f170a428
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134810"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a>使用 Microsoft Graph 将数据写入 Excel 工作簿

Excel REST API 提供了一种简单的、独立于平台的方法将信息上传到 Excel 工作簿。 本主题介绍如何在三个 Web 开发框架上将简单数据集写入 Excel 工作簿：ASP.NET、Angular 和 React。 你可以通过访问 [GitHub 上的 Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter)来查看本主题所采用的代码示例。

> **注意：** 这三个示例将数据写入名为 **demo.xlsx** 的 Excel 工作簿。 它们都提供了此工作簿，以便你可以将其上传到你自己的 OneDrive，不过，你也可以使用 Microsoft Graph 将文件上传到 OneDrive。 如果有意了解 REST 调用，你需要将任何类型的文件上传到你的 OneDrive 根文件夹，请参阅 [Microsoft Graph Excel REST API ASP.NET 待办事项列表示例](https://github.com/microsoftgraph/aspnet-todo-rest-sample)。

这三个 Excel 入门版示例均执行相同的操作：检索登录用户的名称和地址，并将这两条信息添加到 demo.xlsx 工作簿中的新行。 你可以通过将信息添加到代表你想要添加的一行或多行的二维数组中来修改示例，以添加额外的行。

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a>使用单个 REST 请求将一行或多行添加到 Excel 工作簿

Excel REST API 要求将简单的请求正文发布到代表 Excel 工作簿行集合的 REST 终结点。 如果你正在使用登录用户 OneDrive 帐户根文件夹中的笔记本，REST 终结点将如下所示：

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

有关如何获取 OneDrive 文件夹中文件的详细信息，请参阅我们参考文档中的 [DriveItem 资源类型](/graph/api/resources/driveitem?view=graph-rest-1.0)。

> **注意：** 可以通过将 GET 请求发送到以 `/rows` 结尾的路径部分来查看工作簿的现有行集合。

POST 正文如下所示：

```json
{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}
```

第一个 `index` 参数的值指定要添加到零索引行数组的行的相对位置。 插入行下方的行将会向下移动。 `null` 参数指示将添加到结尾的新行。

第二个 `values` 参数的值是一个二维字符串数组，其中包含要添加的每一行未格式化的值。 示例中的数组仅包含一行，但可以通过添加更多字符串数组添加更多行。

通过将 demo.xlsx 文件上传到 OneDrive 根文件夹并在 [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) 上执行此查询，便可使用你自己的 OneDrive 帐户测试此查询。

这是将数据写入 Excel 工作簿所需了解的全部内容。 你需要了解如何在你自己框架中构造并发出请求，Excel 入门版示例演示了执行此操作的三种不同方式。

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a>将一行或多行添加到 ASP.NET Excel 工作簿

你可以在 [ASP.NET 4.6 Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/aspnet-excelstarter-sample)的 [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) 和 [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) 文件中找到构造和发送请求的 ASP.NET 代码。

`GraphResources.cs` 文件提供了帮助程序类，用于封装从 Microsoft Graph 中检索的用户数据，以及在写入工作簿时将使用的请求正文。

```csharp
public class UserInfo
{
    public string Name { get; set; }
    public string Address { get; set; }

}

public class UserInfoRequest
{
    public string index { get; set; }
    public string[][] values { get; set; }
}
```

`GraphService.cs` 类包含 `AddInfoToExcel` 方法，可用于填充这些类、将请求信息序列化为 JSON 对象，然后将该对象作为 POST 请求正文传递。

```csharp
public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
{
    string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
    using (var client = new HttpClient())
    {
        using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
        {
            // Populate UserInfoRequest object
            string[] userInfo = { name, address  };
            string[][] userInfoArray = { userInfo };
            UserInfoRequest userInfoRequest = new UserInfoRequest();
            userInfoRequest.index = null;
            userInfoRequest.values = userInfoArray;

            // Serialize the information in the UserInfoRequest object
            string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
            request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
            request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
            request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

            using (var response = await client.SendAsync(request))
            {
                if (response.IsSuccessStatusCode)
                {
                    return Resource.Graph_UploadToExcel_Success_Result;
                }
                return response.ReasonPhrase;
            }
        }
    }
}
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a>将一行或多行添加到 Angular Excel 工作簿

你可以在 [Angular Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/angular-excelstarter-sample)的 [home.service.ts 文件](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts)中找到构造和发送请求的 Angular 代码。

由于本示例使用 TypeScript，因此，它利用 [Microsoft Graph JavaScript 客户端库](https://github.com/microsoftgraph/msgraph-sdk-javascript)和 [Microsoft Graph TypeScript 类型](https://github.com/microsoftgraph/msgraph-typescript-typings)。

`home.service.ts` 文件中的 `addInfoToExcel` 函数构造二维字符串数组和包含数组的请求正文。 然后使用 Microsoft Graph JavaScript 客户端库构造和发送请求。 响应以承诺的形式返回。

```typescript
addInfoToExcel(user: MicrosoftGraph.User) {
  const userInfo = [];
  const userEmail = user.mail || user.userPrincipalName;
  userInfo.push([user.displayName, userEmail]);

  const userInfoRequestBody = {
    index: null,
    values: userInfo
  };

  const body = JSON.stringify(userInfoRequestBody);

  var client = this.getClient();
  var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
  return Observable.fromPromise(client
  .api(url)
  .post(body)
  );
}
```

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a>将一行或多行添加到 React Excel 工作簿

你可以在 [React Microsoft Graph Excel 入门版示例](https://github.com/microsoftgraph/react-excelstarter-sample)的 [home.js 文件](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js)中找到构造和发送请求的代码。

`onWriteToExcel` 函数构造二维字符串数组并将其作为请求正文传递。 它使用 [axios](https://www.npmjs.com/package/axios) 发出进行 HTTP 请求。

```typescript
onWriteToExcel() {
  const { token, me } = this.state;

  const myEmailAddress = me.mail || me.userPrincipalName;
  const values = [];

  values.push([me.displayName, myEmailAddress]);

  axios
    .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
      { index: null, values },
      { headers: { Authorization: `Bearer ${token}` }}
    )
    .then(res => {
                    console.log(res);
                    const successMessage = "Successfully wrote your data to demo.xlsx!";
                    this.setState ({ successMessage });
                    })
    .catch(err => console.error(err));
}
```

## <a name="see-also"></a>另请参阅

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [通过 Microsoft Graph 显示 Excel 图表图像](excel-display-chart-image.md)
* [使用 Excel REST API](/graph/api/resources/excel?view=graph-rest-1.0)
