jika ingin menggunakan dataset yg berbentuk file tinggal ganti saja dengan 

df = pd.read_csv('./diabetes_latih.csv')

X_train = df.values
X_train = np.delete(X_train,8, axis=1)

y_train = df['Outcome'].values

df = pd.read_csv('./diabetes_uji.csv')

X_test = df.values
X_test = np.delete(X_test,8,axis=1)

y_test = df['Outcome'].values
